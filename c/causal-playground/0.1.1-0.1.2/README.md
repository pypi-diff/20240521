# Comparing `tmp/causal-playground-0.1.1.tar.gz` & `tmp/causal_playground-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causal-playground-0.1.1.tar", last modified: Fri Apr  5 07:50:41 2024, max compression
+gzip compressed data, was "causal_playground-0.1.2.tar", last modified: Tue May 21 09:45:32 2024, max compression
```

## Comparing `causal-playground-0.1.1.tar` & `causal_playground-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:50:41.582765 causal-playground-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:50:41.582765 causal-playground-0.1.1/CausalPlayground/
--rw-r--r--   0 runner    (1001) docker     (127)    13332 2024-04-05 07:50:37.000000 causal-playground-0.1.1/CausalPlayground/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16041 2024-04-05 07:50:37.000000 causal-playground-0.1.1/CausalPlayground/generators.py
--rw-r--r--   0 runner    (1001) docker     (127)    10288 2024-04-05 07:50:37.000000 causal-playground-0.1.1/CausalPlayground/scm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-04-05 07:50:37.000000 causal-playground-0.1.1/CausalPlayground/scm_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-05 07:50:37.000000 causal-playground-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-05 07:50:41.582765 causal-playground-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-05 07:50:37.000000 causal-playground-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:50:41.582765 causal-playground-0.1.1/causal_playground.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-05 07:50:41.000000 causal-playground-0.1.1/causal_playground.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-05 07:50:41.000000 causal-playground-0.1.1/causal_playground.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 07:50:41.000000 causal-playground-0.1.1/causal_playground.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-05 07:50:41.000000 causal-playground-0.1.1/causal_playground.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-05 07:50:41.000000 causal-playground-0.1.1/causal_playground.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-05 07:50:37.000000 causal-playground-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 07:50:41.582765 causal-playground-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 07:50:41.582765 causal-playground-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-05 07:50:37.000000 causal-playground-0.1.1/tests/test_envs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-04-05 07:50:37.000000 causal-playground-0.1.1/tests/test_graph_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-04-05 07:50:37.000000 causal-playground-0.1.1/tests/test_scm_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:45:32.295711 causal_playground-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:45:32.291711 causal_playground-0.1.2/CausalPlayground/
+-rw-r--r--   0 runner    (1001) docker     (127)    13332 2024-05-21 09:45:21.000000 causal_playground-0.1.2/CausalPlayground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18784 2024-05-21 09:45:21.000000 causal_playground-0.1.2/CausalPlayground/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10288 2024-05-21 09:45:21.000000 causal_playground-0.1.2/CausalPlayground/scm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-05-21 09:45:21.000000 causal_playground-0.1.2/CausalPlayground/scm_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-21 09:45:21.000000 causal_playground-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-21 09:45:32.295711 causal_playground-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-21 09:45:21.000000 causal_playground-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:45:32.295711 causal_playground-0.1.2/causal_playground.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-21 09:45:32.000000 causal_playground-0.1.2/causal_playground.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-21 09:45:32.000000 causal_playground-0.1.2/causal_playground.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:45:32.000000 causal_playground-0.1.2/causal_playground.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-21 09:45:32.000000 causal_playground-0.1.2/causal_playground.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-21 09:45:32.000000 causal_playground-0.1.2/causal_playground.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-21 09:45:21.000000 causal_playground-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 09:45:32.295711 causal_playground-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:45:32.295711 causal_playground-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-05-21 09:45:21.000000 causal_playground-0.1.2/tests/test_envs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-21 09:45:21.000000 causal_playground-0.1.2/tests/test_graph_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8044 2024-05-21 09:45:21.000000 causal_playground-0.1.2/tests/test_scm_gen.py
```

### Comparing `causal-playground-0.1.1/CausalPlayground/__init__.py` & `causal_playground-0.1.2/CausalPlayground/__init__.py`

 * *Files identical despite different names*

### Comparing `causal-playground-0.1.1/CausalPlayground/generators.py` & `causal_playground-0.1.2/CausalPlayground/generators.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Tuple, List, Dict, Callable
 from scipy.special import comb
 import copy
 import random
 import networkx as nx
 from tqdm import tqdm
 import pickle
+import dill
 import warnings
 from CausalPlayground import StructuralCausalModel
 
 
 class SCMGenerator:
     """Class for generating SCMs"""
 
@@ -53,14 +54,36 @@
         random.seed(self.seed)
         graph_generator = CausalGraphGenerator(n_endo, n_exo, allow_exo_confounders, seed=self.seed)
         graph, removed_edges = graph_generator.generate_random_graph()
         self.seed += 1
         return self.create_scm_from_graph(graph, possible_functions, exo_distribution, exo_distribution_kwargs),\
                removed_edges
 
+    def create_n_random(self, N: int,  possible_functions: List[str], n_endo: int, n_exo: int, exo_distribution: Callable = None,
+                      exo_distribution_kwargs: dict = None, allow_exo_confounders: bool = False)\
+            -> List[StructuralCausalModel]:
+        """
+        Creates and returns N random StructualCausalModel by calling the create_random function.
+
+        :param N: number of SCMs to generate
+        :param possible_functions: list of function that can be used as causal relations. These should correspond to one
+        of the strings defined in `self.all_functions`.
+        :param n_endo: number of endogenous variables.
+        :param n_exo: number of exogenous variables.
+        :param exo_distribution: distribution of the exogenous variables. This distribution is applied to all
+        exogenous variables.
+        :param exo_distribution_kwargs: keyword arguments for the distribution of exogenous variables
+        :param allow_exo_distribution: true if exogenous confounders should be generated.
+
+        :return: the list of random scms
+        """
+        scms = [self.create_random(possible_functions, n_endo, n_exo, exo_distribution,
+                                   exo_distribution_kwargs, allow_exo_confounders)[0] for _ in range(N)]
+        return scms
+
     def create_scm_from_graph(self, graph: nx.DiGraph, possible_functions: List[str], exo_distribution: Callable,
                               exo_distribution_kwargs: dict) -> StructuralCausalModel:
         """
         Generates an SCM following the structure of a given directed graph. A function is randomly chosen from
         `possible_functions` for each edge in the graph.
 
         :param graph: causal graph
@@ -81,14 +104,50 @@
                 scm.add_endogenous_var(n, self.all_functions[current_function](parents), {p: p for p in parents})
             else:
                 scm.add_exogenous_var(n, exo_distribution, exo_distribution_kwargs)
 
         self.seed += 1
         return scm
 
+    @staticmethod
+    def save_scms(scms: List[StructuralCausalModel], filepath: str, verbose: int = 0) -> None:
+        """
+        Helper function for saving a list of StructuralCausalModels
+        :param scms: list of SCMs for saving
+        :param filepath: path to file for saving the SCMs
+        :param verbose: verbosity level, 0=silent, 1=print to console
+        """
+        try:
+            with open(filepath, 'wb') as file:
+                dill.dump(scms, file)
+            message = f"SCM successfully saved to {filepath}"
+        except IOError as e:
+            message = f"Error saving object to file: {str(e)}"
+        if verbose == 1:
+            print(message)
+
+    @staticmethod
+    def load(filepath: str, verbose: int = 0) -> "StructuralCausalModel":
+        """
+        Helper function for loading SCMs from a file
+        :param filepath: The path and filename of the file to load the object from.
+        :param verbose: verbosity level, 0=silent, 1=print to console
+        :return: the loaded SCMs
+        """
+        try:
+            with open(filepath, 'rb') as file:
+                obj = dill.load(file)
+            return obj
+        except IOError as e:
+            if verbose == 1:
+                print(f"Error loading object from file: {str(e)}")
+        except dill.UnpicklingError as e:
+            if verbose == 1:
+                print(f"Error deserializing object: {str(e)}")
+
 
 class CausalGraphGenerator:
     """Class for generating random directed acyclic graphs."""
 
     allow_exo_confounders: bool
     """flag whether the generated graphs can have exogenous confounders. If False, there will be at most 1 exogenous 
     variable per endogenous variable."""
```

### Comparing `causal-playground-0.1.1/CausalPlayground/scm.py` & `causal_playground-0.1.2/CausalPlayground/scm.py`

 * *Files identical despite different names*

### Comparing `causal-playground-0.1.1/CausalPlayground/scm_environment.py` & `causal_playground-0.1.2/CausalPlayground/scm_environment.py`

 * *Files identical despite different names*

### Comparing `causal-playground-0.1.1/LICENSE` & `causal_playground-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `causal-playground-0.1.1/PKG-INFO` & `causal_playground-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causal-playground
-Version: 0.1.1
+Version: 0.1.2
 Summary: Interactively generating causal data from structural causal models.
 Author-email: Andreas Sauter <a.sauter@vu.nl>
 License: MIT License
 Project-URL: Homepage, https://sa-and.github.io/CausalPlayground/CausalPlayground.html
 Project-URL: Documentation, https://sa-and.github.io/CausalPlayground/CausalPlayground.html
 Project-URL: Repository, https://github.com/sa-and/CausalPlayground
 Keywords: causality,reinforcement learning,structural causal model,data generation,RL,SCM
```

### Comparing `causal-playground-0.1.1/README.md` & `causal_playground-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `causal-playground-0.1.1/causal_playground.egg-info/PKG-INFO` & `causal_playground-0.1.2/causal_playground.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causal-playground
-Version: 0.1.1
+Version: 0.1.2
 Summary: Interactively generating causal data from structural causal models.
 Author-email: Andreas Sauter <a.sauter@vu.nl>
 License: MIT License
 Project-URL: Homepage, https://sa-and.github.io/CausalPlayground/CausalPlayground.html
 Project-URL: Documentation, https://sa-and.github.io/CausalPlayground/CausalPlayground.html
 Project-URL: Repository, https://github.com/sa-and/CausalPlayground
 Keywords: causality,reinforcement learning,structural causal model,data generation,RL,SCM
```

### Comparing `causal-playground-0.1.1/pyproject.toml` & `causal_playground-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "causal-playground"
-version = "0.1.1"
+version = "0.1.2"
 requires-python = ">= 3.10"
 authors = [{name = "Andreas Sauter", email = "a.sauter@vu.nl"}]
 readme = "README.md"
 description = "Interactively generating causal data from structural causal models."
 license = {text = "MIT License"}
 keywords = ["causality", "reinforcement learning", "structural causal model", "data generation", "RL", "SCM"]
 dependencies = [
```

### Comparing `causal-playground-0.1.1/tests/test_envs.py` & `causal_playground-0.1.2/tests/test_envs.py`

 * *Files identical despite different names*

### Comparing `causal-playground-0.1.1/tests/test_graph_gen.py` & `causal_playground-0.1.2/tests/test_graph_gen.py`

 * *Files identical despite different names*

### Comparing `causal-playground-0.1.1/tests/test_scm_gen.py` & `causal_playground-0.1.2/tests/test_scm_gen.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,48 +4,50 @@
 import unittest
 from functions import *
 import random
 import os
 
 
 class TestSCM(unittest.TestCase):
-    def __init__(self, *args,  **kwargs):
+    def __init__(self, *args, **kwargs):
         super(TestSCM, self).__init__(*args, **kwargs)
-        self.scm = SCMGenerator(all_functions={'linear': f_linear}, seed=42).create_random(possible_functions=["linear"], n_endo=20, n_exo=0)[0]
+        self.scm = \
+        SCMGenerator(all_functions={'linear': f_linear}, seed=42).create_random(possible_functions=["linear"],
+                                                                                n_endo=20, n_exo=0)[0]
         self.test_scm = StructuralCausalModel()
         self.test_scm.add_endogenous_var('A', lambda noise: noise + 5, {'noise': 'U'})
         self.test_scm.add_exogenous_var('U', random.randint, {'a': 3, 'b': 8})
         self.test_scm.add_endogenous_var('Effect', lambda x: x * 2, {'x': 'A'})
 
     def test_creation(self):
         sample = self.test_scm.get_next_sample()
         u = sample[1]['U']
         a = sample[0]['A']
         effect = sample[0]['EFFECT']
         self.assertIn(u, [3, 4, 5, 6, 7, 8])
-        self.assertEqual(a, u+5)
-        self.assertEqual(effect, a*2)
+        self.assertEqual(a, u + 5)
+        self.assertEqual(effect, a * 2)
 
     def test_create_from_graph(self):
         graph = self.test_scm.create_graph()
         generator = SCMGenerator(all_functions={'linear': f_linear}, seed=1)
         scm = generator.create_scm_from_graph(graph=graph, possible_functions=['linear'],
                                               exo_distribution=random.randint, exo_distribution_kwargs={'a': 2, 'b': 5})
         self.assertTrue(scm.functions['A'][1] == {'U': 'U'})
         sample = scm.get_next_sample()
         u = sample[1]['U']
         a = sample[0]['A']
         effect = sample[0]['EFFECT']
         self.assertIn(u, [2, 3, 4, 5])
-        self.assertTrue(effect <= 2*a)
-    
+        self.assertTrue(effect <= 2 * a)
+
     def test_intervention(self):
         # do an intervention and compare before and after
         x0 = self.scm.get_next_sample()[0]['X0']
-        self.scm.do_interventions([("X0", (lambda: 5, {})), ("X1", (lambda x0: x0+1, {'x0': 'X0'}))])
+        self.scm.do_interventions([("X0", (lambda: 5, {})), ("X1", (lambda x0: x0 + 1, {'x0': 'X0'}))])
         x0_do = self.scm.get_next_sample()[0]['X0']
         x1_do = self.scm.get_next_sample()[0]['X1']
         self.assertTrue(x0_do == 5)
         self.assertTrue(x1_do == 6)
         self.assertFalse(x0 == x0_do)
 
         # test graphical implications
@@ -86,19 +88,28 @@
         self.assertEqual(list(loaded_scm.endogenous_vars.keys()), ['A', 'EFFECT'])
         self.assertEqual(list(loaded_scm.exogenous_vars.keys()), ['U'])
         self.assertEqual(loaded_scm.create_graph().edges, self.test_scm.create_graph().edges)
 
         if os.path.exists("./delme.pkl"):
             os.remove("./delme.pkl")
 
+    def test_create_n_random(self):
+        generator = SCMGenerator(all_functions={'linear': f_linear}, seed=1)
+        scms = generator.create_n_random(10, ['linear'], 3, 4,
+                                         random.random, {}, False)
+        self.assertTrue(len(scms) == 10)
+        self.assertTrue(type(scms[0]) == StructuralCausalModel)
+
 
 class TestRandNN(unittest.TestCase):
-    def __init__(self, *args,  **kwargs):
+    def __init__(self, *args, **kwargs):
         super(TestRandNN, self).__init__(*args, **kwargs)
-        self.scm1 = SCMGenerator(all_functions={'linear': f_linear}, seed=42).create_random(possible_functions=["linear"], n_endo=10, n_exo=0)[0]
+        self.scm1 = \
+        SCMGenerator(all_functions={'linear': f_linear}, seed=42).create_random(possible_functions=["linear"],
+                                                                                n_endo=10, n_exo=0)[0]
         # self.scm2 = SCMGenerator(seed=42).create_random(possible_functions=["NN"], n_endo=6, n_exo=8,
         #                                                 exo_distribution=random.random, exo_distribution_kwargs={})[0]
 
     def test_sampling_types(self):
         vals = self.scm1.get_next_sample()[0]
         self.assertTrue(isinstance(vals['X0'], float))
         self.assertTrue(len(vals) == 10)
@@ -153,7 +164,8 @@
         sample2 = self.scm_unconfounded.get_next_sample()
         self.assertNotEqual(list(sample1[0].values()), list(sample2[0].values()))  # endogenous vars
         self.assertNotEqual(list(sample1[1].values()), list(sample2[1].values()))  # exoogenous vars
 
 
 if __name__ == '__main__':
     unittest.main()
+
```

