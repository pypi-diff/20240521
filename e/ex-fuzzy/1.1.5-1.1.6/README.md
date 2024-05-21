# Comparing `tmp/ex_fuzzy-1.1.5.tar.gz` & `tmp/ex_fuzzy-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ex_fuzzy-1.1.5.tar", last modified: Wed Apr 24 14:44:20 2024, max compression
+gzip compressed data, was "ex_fuzzy-1.1.6.tar", last modified: Tue May 21 15:50:10 2024, max compression
```

## Comparing `ex_fuzzy-1.1.5.tar` & `ex_fuzzy-1.1.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 14:44:20.570669 ex_fuzzy-1.1.5/
--rw-rw-rw-   0        0        0    35184 2024-04-10 13:18:52.000000 ex_fuzzy-1.1.5/LICENSE
--rw-rw-rw-   0        0        0     4333 2024-04-24 14:44:20.563668 ex_fuzzy-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     3284 2024-04-22 14:14:00.000000 ex_fuzzy-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 14:44:20.446658 ex_fuzzy-1.1.5/ex_fuzzy/
-drwxrwxrwx   0        0        0        0 2024-04-24 14:44:20.536666 ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/
--rw-rw-rw-   0        0        0      282 2024-04-05 15:43:34.000000 ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/__init__.py
--rw-rw-rw-   0        0        0     6197 2024-01-31 12:48:36.000000 ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/centroid.py
--rw-rw-rw-   0        0        0    11027 2024-04-11 15:17:33.000000 ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/classifiers.py
--rw-rw-rw-   0        0        0     7433 2024-01-30 16:48:50.000000 ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/cognitive_maps.py
--rw-rw-rw-   0        0        0    15878 2024-04-18 15:39:28.000000 ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/eval_rules.py
--rw-rw-rw-   0        0        0     2693 2024-04-24 13:08:01.000000 ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/eval_tools.py
--rw-rw-rw-   0        0        0    43114 2024-04-24 13:36:10.000000 ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/evolutionary_fit.py
--rw-rw-rw-   0        0        0    17306 2024-04-05 15:07:12.000000 ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/fuzzy_sets.py
--rw-rw-rw-   0        0        0     6160 2024-04-03 14:16:49.000000 ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/maintenance.py
--rw-rw-rw-   0        0        0     3677 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/persistence.py
--rw-rw-rw-   0        0        0    11420 2024-04-05 16:05:24.000000 ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/rule_mining.py
--rw-rw-rw-   0        0        0    41199 2024-04-23 15:06:45.000000 ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/rules.py
--rw-rw-rw-   0        0        0    27001 2024-01-31 15:05:05.000000 ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/temporal.py
--rw-rw-rw-   0        0        0    25751 2024-04-05 15:33:36.000000 ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/utils.py
--rw-rw-rw-   0        0        0    16171 2024-04-24 14:42:34.000000 ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/vis_rules.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:44:20.478662 ex_fuzzy-1.1.5/ex_fuzzy.egg-info/
--rw-rw-rw-   0        0        0     4333 2024-04-24 14:44:20.000000 ex_fuzzy-1.1.5/ex_fuzzy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      785 2024-04-24 14:44:20.000000 ex_fuzzy-1.1.5/ex_fuzzy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 14:44:20.000000 ex_fuzzy-1.1.5/ex_fuzzy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-04-24 14:44:20.000000 ex_fuzzy-1.1.5/ex_fuzzy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-24 14:44:20.000000 ex_fuzzy-1.1.5/ex_fuzzy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 14:44:20.572668 ex_fuzzy-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1773 2024-04-24 14:44:15.000000 ex_fuzzy-1.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-24 14:44:20.555672 ex_fuzzy-1.1.5/tests/
--rw-rw-rw-   0        0        0     1261 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.5/tests/test_centroids.py
--rw-rw-rw-   0        0        0     1963 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.5/tests/test_classification.py
--rw-rw-rw-   0        0        0      797 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.5/tests/test_eval_tools.py
--rw-rw-rw-   0        0        0     1821 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.5/tests/test_fuzzy_sets.py
--rw-rw-rw-   0        0        0     4189 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.5/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:50:10.714138 ex_fuzzy-1.1.6/
+-rw-rw-rw-   0        0        0    35184 2024-04-10 13:18:52.000000 ex_fuzzy-1.1.6/LICENSE
+-rw-rw-rw-   0        0        0     4185 2024-05-21 15:50:10.714138 ex_fuzzy-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3284 2024-04-22 14:14:00.000000 ex_fuzzy-1.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 15:50:10.658262 ex_fuzzy-1.1.6/ex_fuzzy/
+drwxrwxrwx   0        0        0        0 2024-05-21 15:50:10.707284 ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/
+-rw-rw-rw-   0        0        0      282 2024-04-05 15:43:34.000000 ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/__init__.py
+-rw-rw-rw-   0        0        0     6197 2024-01-31 12:48:36.000000 ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/centroid.py
+-rw-rw-rw-   0        0        0    11027 2024-04-11 15:17:33.000000 ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/classifiers.py
+-rw-rw-rw-   0        0        0     7433 2024-01-30 16:48:50.000000 ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/cognitive_maps.py
+-rw-rw-rw-   0        0        0    15878 2024-04-18 15:39:28.000000 ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/eval_rules.py
+-rw-rw-rw-   0        0        0     2693 2024-04-24 13:08:01.000000 ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/eval_tools.py
+-rw-rw-rw-   0        0        0    43154 2024-05-20 11:58:00.000000 ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/evolutionary_fit.py
+-rw-rw-rw-   0        0        0    18159 2024-05-07 18:39:25.000000 ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/fuzzy_sets.py
+-rw-rw-rw-   0        0        0     6160 2024-04-03 14:16:49.000000 ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/maintenance.py
+-rw-rw-rw-   0        0        0     3677 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/persistence.py
+-rw-rw-rw-   0        0        0    11420 2024-04-05 16:05:24.000000 ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/rule_mining.py
+-rw-rw-rw-   0        0        0    41778 2024-05-21 15:45:06.000000 ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/rules.py
+-rw-rw-rw-   0        0        0    27001 2024-01-31 15:05:05.000000 ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/temporal.py
+-rw-rw-rw-   0        0        0    26136 2024-05-06 15:11:07.000000 ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/utils.py
+-rw-rw-rw-   0        0        0    16171 2024-04-24 14:42:34.000000 ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/vis_rules.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:50:10.691594 ex_fuzzy-1.1.6/ex_fuzzy.egg-info/
+-rw-rw-rw-   0        0        0     4185 2024-05-21 15:50:10.000000 ex_fuzzy-1.1.6/ex_fuzzy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      785 2024-05-21 15:50:10.000000 ex_fuzzy-1.1.6/ex_fuzzy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 15:50:10.000000 ex_fuzzy-1.1.6/ex_fuzzy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-05-21 15:50:10.000000 ex_fuzzy-1.1.6/ex_fuzzy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-21 15:50:10.000000 ex_fuzzy-1.1.6/ex_fuzzy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 15:50:10.714138 ex_fuzzy-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1773 2024-05-21 15:49:10.000000 ex_fuzzy-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:50:10.713136 ex_fuzzy-1.1.6/tests/
+-rw-rw-rw-   0        0        0     1261 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.6/tests/test_centroids.py
+-rw-rw-rw-   0        0        0     1963 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.6/tests/test_classification.py
+-rw-rw-rw-   0        0        0      797 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.6/tests/test_eval_tools.py
+-rw-rw-rw-   0        0        0     1821 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.6/tests/test_fuzzy_sets.py
+-rw-rw-rw-   0        0        0     4189 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.6/tests/test_utils.py
```

### Comparing `ex_fuzzy-1.1.5/LICENSE` & `ex_fuzzy-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.5/PKG-INFO` & `ex_fuzzy-1.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ex_fuzzy
-Version: 1.1.5
+Version: 1.1.6
 Summary: Library to perform explainable AI using fuzzy logic.
 Home-page: https://github.com/Fuminides/ex-fuzzy
 Download-URL: https://pypi.org/project/ex-fuzzy/
 Maintainer: Javier Fumanal Idocin
 Maintainer-email: javierfumanalidocin@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
@@ -14,20 +14,14 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: networkx
-Requires-Dist: matplotlib
-Requires-Dist: pymoo
-Requires-Dist: pandas
-Requires-Dist: scikit-learn
 
 # Ex-Fuzzy
 ex-Fuzzy is a fuzzy toolbox library for Python with special focus in its accesibility to use and visualization of results. In this way, we focus on the ex(-Fuzzy)plainable capacities of approximate reasoning.
 
 Some of the tools available in this library include:
 
 - Support for approximate reasoning using fuzzy association rules, for both classification and regression problems. This includes rule base optimization using genetic algorithms and rule visualization.
```

### Comparing `ex_fuzzy-1.1.5/README.md` & `ex_fuzzy-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/centroid.py` & `ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/centroid.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/classifiers.py` & `ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/classifiers.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/cognitive_maps.py` & `ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/cognitive_maps.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/eval_rules.py` & `ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/eval_rules.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/eval_tools.py` & `ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/eval_tools.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/evolutionary_fit.py` & `ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/evolutionary_fit.py`

 * *Files 0% similar despite different names*

```diff
@@ -833,15 +833,15 @@
 
                 init_rule_antecedents[ant] = antecedent_parameters[jx]
 
             consequent_idx = x[fourth_pointer + aux_pointer]
             assert consequent_idx < self.n_classes, "Consequent class is not valid. Something in the gene is wrong."
             aux_pointer += 1
  
-            if consequent_idx != -1:
+            if consequent_idx != -1 and np.any(init_rule_antecedents != -1):
                 rule_list[consequent_idx].append(
                     rules.RuleSimple(init_rule_antecedents, 0))
 
         # If we optimize the membership functions
         if self.lvs is None:
             third_pointer = 2 * self.nAnts * self.nRules
             aux_pointer = 0
```

### Comparing `ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/fuzzy_sets.py` & `ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/fuzzy_sets.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,73 @@
 """
 This is a the source file that contains the class of GT2 fuzzy set and its most direct applications, 
 like computing the FM function, etc.
 
 """
 import enum
+from typing import Generator
 
 import numpy as np
 
 try:
     from . import maintenance as mnt
 except:
     import maintenance as mnt
 
+# You dont require torch to use this module, however, we need to import it to give support in case you feed these methods with torch tensors.
+try:
+    import torch
+    torch_available = True
+except:
+    torch_available = False
+
 
 ''' Enum that defines the fuzzy set types.'''
 class FUZZY_SETS(enum.Enum):
     t1 = 'Type 1'
     t2 = 'Type 2'
     gt2 = 'General Type 2'
 
 
     def __eq__(self, __value: object) -> bool:
         return self.value == __value.value
 
+
 def trapezoidal_membership(x: np.array, params: list[float], epsilon=10E-5) -> np.array:
     '''
     Trapezoidal membership functions.
 
     :param x: input values in the fuzzy set referencial domain.
     :param params:  four numbers that comprises the start and end of the trapezoid.
     :param epsilon: small float number for numerical stability. Adjust accordingly only if there are NaN issues.
     '''
     a, b, c, d = params
 
     # Special case: a singleton trapezoid
     if a == d:
-        return np.equal(a, x).astype(float)
+        # If they are numpy arrays, we need to use the numpy function
+        if isinstance(x, np.ndarray):
+            return np.equal(x, a).astype(float)
+        if torch_available:
+            if isinstance(x, torch.Tensor):
+                return torch.eq(x, a).float()
+            
 
     if b == a:
         b += epsilon
     if c == d:
         d += epsilon
 
     aux1 = (x - a) / (b - a)
     aux2 = (d - x) / (d - c)
 
-    return np.clip(np.minimum(aux1, aux2), 0.0, 1.0)
+    if isinstance(x, np.ndarray):
+        return np.clip(np.minimum(aux1, aux2), 0.0, 1.0)
+    elif isinstance(x, torch.Tensor):
+        return torch.clamp(torch.min(aux1, aux2), 0.0, 1.0)
 
 
 def __gaussian2(x, params: list[float]) -> np.array:
     '''
     Gaussian membership functions.
 
     :param mean:  real number, mean of the gaussian function.
@@ -130,15 +148,19 @@
 
     def membership(self, x: np.array) -> np.array:
         '''
         Computes the membership of a point or vector of elements.
 
         :param x: input values in the referencial domain.
         '''
-        res = np.equal(x, self.category).astype(float)
+        if isinstance(x, np.ndarray):
+            res = np.equal(x, self.category).astype(float)
+        if torch_available:
+            if isinstance(x, torch.Tensor):
+                res = torch.eq(x, self.category).float()
 
         return res
 
 
     def type(self) -> FUZZY_SETS:
         '''
         Returns the corresponding fuzzy set type according to FUZZY_SETS enum.
@@ -485,15 +507,15 @@
 
         :param item: int. Index of the FS.
         :param elem: FS. The FS to set.
         '''
         self.linguistic_variables[item] = elem
     
 
-    def __iter__(self) -> FS:
+    def __iter__(self) -> Generator[FS, None, None]:
         '''
         Returns the corresponding fs.
 
         :param item: int. Index of the FS.
         :return: FS. The corresponding FS.
         '''
         for fs in self.linguistic_variables:
```

### Comparing `ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/maintenance.py` & `ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/maintenance.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/persistence.py` & `ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/persistence.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/rule_mining.py` & `ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/rule_mining.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/rules.py` & `ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/rules.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,14 +115,15 @@
         Creates a rule with the given antecedents and consequent.
 
         :param antecedents: list of integers indicating the linguistic variable used for each input.
         :param consequent: integer indicating the linguistic variable used for the consequent.
         '''
         self.antecedents = list(map(int, antecedents))
         self.consequent = int(consequent)
+        self.score = 1.0
 
 
     def __getitem__(self, ix):
         '''
         Returns the antecedent value for the given index.
 
         :param ix: index of the antecedent to return.
@@ -183,29 +184,31 @@
         :param tnorm: t-norm to use in the inference process.
         '''
         rules = self.delete_rule_duplicates(rules)
         self.rules = rules
         self.antecedents = antecedents
         self.consequent = consequent
         self.tnorm = tnorm
-        self.consequent_centroids = np.zeros(
-            (len(consequent.linguistic_variable_names()), 2))
-        for ix, vl_consequent in enumerate(consequent.linguistic_variables):
-            consequent_domain = vl_consequent.domain
-            domain_linspace = np.arange(
-                consequent_domain[0], consequent_domain[1], 0.05)
-            consequent_memberships = vl_consequent.membership(domain_linspace)
 
-            self.consequent_centroids[ix, :] = centroid.compute_centroid_iv(
-                domain_linspace, consequent_memberships)
+        if consequent is not None:
+            self.consequent_centroids = np.zeros(
+                (len(consequent.linguistic_variable_names()), 2))
+            for ix, vl_consequent in enumerate(consequent.linguistic_variables):
+                consequent_domain = vl_consequent.domain
+                domain_linspace = np.arange(
+                    consequent_domain[0], consequent_domain[1], 0.05)
+                consequent_memberships = vl_consequent.membership(domain_linspace)
 
-        self.consequent_centroids_rules = np.zeros((len(self.rules), 2))
-        for ix, rule in enumerate(self.rules):
-            consequent_ix = rule.consequent
-            self.consequent_centroids_rules[ix] = self.consequent_centroids[consequent_ix]
+                self.consequent_centroids[ix, :] = centroid.compute_centroid_iv(
+                    domain_linspace, consequent_memberships)
+
+            self.consequent_centroids_rules = np.zeros((len(self.rules), 2))
+            for ix, rule in enumerate(self.rules):
+                consequent_ix = rule.consequent
+                self.consequent_centroids_rules[ix] = self.consequent_centroids[consequent_ix]
 
         self.delete_duplicates()
 
 
     def get_rules(self) -> list[RuleSimple]:
         '''
         Returns the list of rules in the rulebase.
@@ -341,17 +344,16 @@
                 membership = np.zeros((x.shape[0], len(rule_antecedents)))
             elif self.fuzzy_type() == fs.FUZZY_SETS.t2:
                 membership = np.zeros((x.shape[0], len(rule_antecedents), 2))
             elif self.fuzzy_type() == fs.FUZZY_SETS.gt2:
                 membership = np.zeros(
                     (x.shape[0], len(rule_antecedents), len(self.alpha_cuts), 2))
 
-            
+            n_nonvl = 0
             for ix, vl in enumerate(rule_antecedents):
-                n_nonvl = 0
                 if vl >= 0:
                     membership_antecedent = list(antecedents_memberships[ix])[vl]
                     membership[:, ix] = membership_antecedent
                     n_nonvl += 1
                 else:
                     membership[:, ix] = 1.0
 
@@ -488,16 +490,20 @@
         delete_list = []
         try:
             for ix, rule in enumerate(self.rules):
                 score = rule.score
                 if (self.fuzzy_type() == fs.FUZZY_SETS.t2) or (self.fuzzy_type() == fs.FUZZY_SETS.gt2):
                     score = np.mean(score)
 
-                if score < tolerance or rule.accuracy == 0.0:
-                    delete_list.append(ix)
+                try:
+                    if score < tolerance or rule.accuracy == 0.0:
+                        delete_list.append(ix)
+                except AttributeError:
+                    if score < tolerance:
+                        delete_list.append(ix)
         except AttributeError:
             assert False, 'Dominance scores not computed for this rulebase'
 
         self.remove_rules(delete_list)
 
 
     def scores(self) -> np.array:
@@ -1126,23 +1132,28 @@
 
     :param rule_matrix: matrix with the rules.
     :param consequents: array with the consequents per rule.
     :param antecedents: list of fuzzy variables.
     :param class_names: list with the names of the classes.
     '''
     rule_lists = {ix:[] for ix in range(len(np.unique(consequents)))}
-
+    fs_studied = antecedents[0].fuzzy_type()
     for ix, consequent in enumerate(consequents):
-        if not np.equal(rule_matrix, -1).all():
+        if not np.equal(rule_matrix[ix], -1).all():
             rule_object = RuleSimple(rule_matrix[ix])
             rule_object.score = rule_weights[ix]
             rule_lists[consequent].append(rule_object)
 
     for ix, consequent in enumerate(np.unique(consequents)):
-        rule_base = RuleBaseT1(antecedents, rule_lists[ix])
+        if fs_studied == fs.FUZZY_SETS.t1:
+            rule_base = RuleBaseT1(antecedents, rule_lists[ix])
+        elif fs_studied == fs.FUZZY_SETS.t2:
+            rule_base = RuleBaseT2(antecedents, rule_lists[ix])
+        elif fs_studied == fs.FUZZY_SETS.gt2:
+            rule_base = RuleBaseGT2(antecedents, rule_lists[ix])
         
         if ix == 0:
             res = MasterRuleBase([rule_base], np.unique(consequents))
         else:
             res.add_rule_base(rule_base)
 
     if class_names is not None:
```

### Comparing `ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/temporal.py` & `ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/temporal.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/utils.py` & `ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,16 +60,14 @@
 def t1_simple_partition(x: np.array) -> np.array:
     '''
     Partitions the fuzzy variable in four trapezoidal memberships.
 
     :param x: numpy array, vector of shape (samples, ).
     :return: numpy array, vector of shape (variables, 4, 4).
     '''
-    
-
     n_partitions = 4
     trap_memberships_size = 4
     quantile_numbers = fixed_quantile_compute(x)
 
     partition_parameters = np.zeros(
         (x.shape[1], n_partitions, trap_memberships_size))
     for partition in range(n_partitions):
@@ -295,17 +293,23 @@
     :param fz_type_studied: fuzzy set type studied.
     :param categorial_mask: a boolean mask vector that indicates for each variables if its categorical or not.
     '''
     if mnt.save_usage_flag:
         mnt.usage_data[mnt.usage_categories.Funcs]['precompute_labels'] += 1
         mnt.usage_data[mnt.usage_categories.FuzzySets][fz_type_studied.name] += 1
 
+    if isinstance(X, pd.DataFrame):
+        feat_names = X.columns
+        X = X.values
+    else:
+        feat_names = [str(ix) for ix in range(X.shape[1])]
+
     # Get the X dataframe without the categorical variables
     if categorical_mask is not None:
-        X_numerical = X.loc[:, np.array(~categorical_mask)]
+        X_numerical = X[:, np.logical_not(categorical_mask)]
     else:
         X_numerical = X
 
     if fz_type_studied == fs.FUZZY_SETS.t1:
         precomputed_partitions = t1_fuzzy_partitions_dataset(X_numerical)
     elif fz_type_studied == fs.FUZZY_SETS.t2:
         precomputed_partitions = t2_fuzzy_partitions_dataset(X_numerical)
@@ -319,26 +323,35 @@
             if elem:
                 if isinstance(X, pd.DataFrame):
                     name = X.columns[ix]
                 else:
                     name = str(ix)
                 cat_var = construct_crisp_categorical_partition(np.array(X)[:, ix], name, fz_type_studied)
 
-                categorical_partition[X.columns[ix]] = cat_var
+                categorical_partition[name] = cat_var
 
         # Reorder the partitions so that they follow the same order as in the original X
         precomputed_partitions_aux = []
         for ix, elem in enumerate(categorical_mask):
+            if isinstance(X, pd.DataFrame):
+                name = X.columns[ix]
+            else:
+                name = str(ix)
+
             if elem:
-                precomputed_partitions_aux.append(categorical_partition[X.columns[ix]])
+                precomputed_partitions_aux.append(categorical_partition[name])
             else:
                 precomputed_partitions_aux.append(precomputed_partitions.pop(0))
 
         precomputed_partitions = precomputed_partitions_aux
 
+    
+    for ix, partition in enumerate(precomputed_partitions):
+        partition.name = feat_names[ix]
+
     return precomputed_partitions
 
 
 def construct_crisp_categorical_partition(x: np.array, name: str, fz_type_studied: fs.FUZZY_SETS) -> fs.fuzzyVariable:
     '''
     Creates a fuzzy variable for a categorical feature.
```

### Comparing `ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/vis_rules.py` & `ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/vis_rules.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.5/ex_fuzzy.egg-info/PKG-INFO` & `ex_fuzzy-1.1.6/ex_fuzzy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ex-fuzzy
-Version: 1.1.5
+Version: 1.1.6
 Summary: Library to perform explainable AI using fuzzy logic.
 Home-page: https://github.com/Fuminides/ex-fuzzy
 Download-URL: https://pypi.org/project/ex-fuzzy/
 Maintainer: Javier Fumanal Idocin
 Maintainer-email: javierfumanalidocin@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
@@ -14,20 +14,14 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: networkx
-Requires-Dist: matplotlib
-Requires-Dist: pymoo
-Requires-Dist: pandas
-Requires-Dist: scikit-learn
 
 # Ex-Fuzzy
 ex-Fuzzy is a fuzzy toolbox library for Python with special focus in its accesibility to use and visualization of results. In this way, we focus on the ex(-Fuzzy)plainable capacities of approximate reasoning.
 
 Some of the tools available in this library include:
 
 - Support for approximate reasoning using fuzzy association rules, for both classification and regression problems. This includes rule base optimization using genetic algorithms and rule visualization.
```

### Comparing `ex_fuzzy-1.1.5/ex_fuzzy.egg-info/SOURCES.txt` & `ex_fuzzy-1.1.6/ex_fuzzy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.5/setup.py` & `ex_fuzzy-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 DISTNAME = "ex_fuzzy"
 DESCRIPTION = "Library to perform explainable AI using fuzzy logic."
 MAINTAINER = "Javier Fumanal Idocin"
 MAINTAINER_EMAIL = "javierfumanalidocin@gmail.com"
 URL = "https://github.com/Fuminides/ex-fuzzy"
 LICENSE = "GPL-3.0"
 DOWNLOAD_URL = "https://pypi.org/project/ex-fuzzy/"
-VERSION = "1.1.5"
+VERSION = "1.1.6"
 INSTALL_REQUIRES = ["numpy", "networkx", "matplotlib", "pymoo", "pandas", "scikit-learn"]
 CLASSIFIERS = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.7",
```

### Comparing `ex_fuzzy-1.1.5/tests/test_centroids.py` & `ex_fuzzy-1.1.6/tests/test_centroids.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.5/tests/test_classification.py` & `ex_fuzzy-1.1.6/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.5/tests/test_eval_tools.py` & `ex_fuzzy-1.1.6/tests/test_eval_tools.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.5/tests/test_fuzzy_sets.py` & `ex_fuzzy-1.1.6/tests/test_fuzzy_sets.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.5/tests/test_utils.py` & `ex_fuzzy-1.1.6/tests/test_utils.py`

 * *Files identical despite different names*

