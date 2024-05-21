# Comparing `tmp/module_sdstate-0.1.2.tar.gz` & `tmp/module_sdstate-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "module_sdstate-0.1.2.tar", max compression
+gzip compressed data, was "module_sdstate-0.1.3.tar", max compression
```

## Comparing `module_sdstate-0.1.2.tar` & `module_sdstate-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1092 2024-02-23 19:52:24.045015 module_sdstate-0.1.2/LICENSE
--rw-r--r--   0        0        0      680 2024-05-06 20:46:09.395470 module_sdstate-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1162 2024-02-26 20:26:54.627700 module_sdstate-0.1.2/README.md
--rw-r--r--   0        0        0      118 2024-02-26 20:20:38.191958 module_sdstate-0.1.2/src/module_sdstate/__init__.py
--rw-r--r--   0        0        0     6603 2024-05-06 20:37:26.351098 module_sdstate-0.1.2/src/module_sdstate/lanczos_utils.py
--rw-r--r--   0        0        0    10149 2024-02-26 20:19:06.196762 module_sdstate-0.1.2/src/module_sdstate/sdstate_utils.py
--rw-r--r--   0        0        0     2010 1970-01-01 00:00:00.000000 module_sdstate-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-02-23 19:52:24.045015 module_sdstate-0.1.3/LICENSE
+-rw-r--r--   0        0        0      680 2024-05-21 21:30:05.142896 module_sdstate-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1162 2024-02-26 20:26:54.627700 module_sdstate-0.1.3/README.md
+-rw-r--r--   0        0        0      118 2024-02-26 20:20:38.191958 module_sdstate-0.1.3/src/module_sdstate/__init__.py
+-rw-r--r--   0        0        0     6603 2024-05-06 20:37:26.351098 module_sdstate-0.1.3/src/module_sdstate/lanczos_utils.py
+-rw-r--r--   0        0        0    10302 2024-05-21 21:27:44.095415 module_sdstate-0.1.3/src/module_sdstate/sdstate_utils.py
+-rw-r--r--   0        0        0     2010 1970-01-01 00:00:00.000000 module_sdstate-0.1.3/PKG-INFO
```

### Comparing `module_sdstate-0.1.2/LICENSE` & `module_sdstate-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `module_sdstate-0.1.2/pyproject.toml` & `module_sdstate-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "module_sdstate"
-version = "0.1.2"
+version = "0.1.3"
 description = "Implementation of Slater Determinant states as dictionaries of states and coefficient pairs. Each state is represented with an integar treated as binary, allowing applying of Excitation operators on the state efficiently. Memory-efficient implementation of Lanczos iteration for estimating Hamiltonian spectrum range."
 authors = ["Linjun Wang"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `module_sdstate-0.1.2/README.md` & `module_sdstate-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `module_sdstate-0.1.2/src/module_sdstate/lanczos_utils.py` & `module_sdstate-0.1.3/src/module_sdstate/lanczos_utils.py`

 * *Files identical despite different names*

### Comparing `module_sdstate-0.1.2/src/module_sdstate/sdstate_utils.py` & `module_sdstate-0.1.3/src/module_sdstate/sdstate_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -155,15 +155,19 @@
         n2 = st.n_qubit
         n = self.n_qubit + st.n_qubit
         tmp = sdstate(n_qubit = n)
         for s1 in self.dic:
             for s2 in st.dic:
                 tmp += sdstate(s = s1 << n2 | s2, coeff = self.dic[s1] * st.dic[s2], n_qubit = n)
         return tmp
-                
+    
+    def truncate(self, n):
+#         Truncate the state, leaving only the n states of leading coefficients
+        self.dic = dict(sorted(self.dic.items(), key=lambda item: abs(item[1]), reverse=True)[:n])
+    
     def Epq(self, p, q):
         """
         Return the action of a_p^a_q on the current state.
         """
         tmp = sdstate(n_qubit = self.n_qubit)
         for n in self.dic:
             if actable_pq(n, p, q):
@@ -194,15 +198,14 @@
         return partial_state
     
     def Hf_state(self, Hf: of.FermionOperator, multiprocessing = False):
         """Apply a Hamiltonian in FermionOperator on the current state. multiprocessing can be used
         to parallelize the process of applying each Excitation operator in the Hamiltonian. The general
         cost is given by O(N^4M), for N as the qubit dimension and M as the size of the current state.
         """
-        H = of.transforms.chemist_ordered(Hf)
         re_state = sdstate(n_qubit = self.n_qubit)
         if multiprocessing:
             # Convert FermionOperator terms to a list of tuples for easy batch processing
             terms_list = [(t, H.terms[t]) for t in H.terms]
 
             # Determine the optimal number of batches
             num_processes = min(len(terms_list), os.cpu_count())
```

### Comparing `module_sdstate-0.1.2/PKG-INFO` & `module_sdstate-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: module_sdstate
-Version: 0.1.2
+Version: 0.1.3
 Summary: Implementation of Slater Determinant states as dictionaries of states and coefficient pairs. Each state is represented with an integar treated as binary, allowing applying of Excitation operators on the state efficiently. Memory-efficient implementation of Lanczos iteration for estimating Hamiltonian spectrum range.
 License: MIT
 Author: Linjun Wang
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

