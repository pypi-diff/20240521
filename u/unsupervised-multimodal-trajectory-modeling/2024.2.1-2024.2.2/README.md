# Comparing `tmp/unsupervised-multimodal-trajectory-modeling-2024.2.1.tar.gz` & `tmp/unsupervised_multimodal_trajectory_modeling-2024.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unsupervised-multimodal-trajectory-modeling-2024.2.1.tar", last modified: Wed Mar 13 15:16:52 2024, max compression
+gzip compressed data, was "unsupervised_multimodal_trajectory_modeling-2024.2.2.tar", last modified: Tue May 21 15:03:53 2024, max compression
```

## Comparing `unsupervised-multimodal-trajectory-modeling-2024.2.1.tar` & `unsupervised_multimodal_trajectory_modeling-2024.2.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-13 15:16:52.468924 unsupervised-multimodal-trajectory-modeling-2024.2.1/
--rw-r--r--   0 michael    (501) staff       (20)     1070 2024-02-20 16:14:41.000000 unsupervised-multimodal-trajectory-modeling-2024.2.1/LICENSE.txt
--rw-r--r--   0 michael    (501) staff       (20)     9296 2024-03-13 15:16:52.468676 unsupervised-multimodal-trajectory-modeling-2024.2.1/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)     6851 2024-03-01 18:30:51.000000 unsupervised-multimodal-trajectory-modeling-2024.2.1/README.md
--rw-r--r--   0 michael    (501) staff       (20)     1407 2024-03-13 15:01:39.000000 unsupervised-multimodal-trajectory-modeling-2024.2.1/pyproject.toml
--rw-r--r--   0 michael    (501) staff       (20)       38 2024-03-13 15:16:52.468970 unsupervised-multimodal-trajectory-modeling-2024.2.1/setup.cfg
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-13 15:16:52.461254 unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling/
--rw-r--r--   0 michael    (501) staff       (20)        0 2024-03-04 01:36:58.000000 unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling/__init__.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-13 15:16:52.463602 unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling/linear_gaussian/
--rw-r--r--   0 michael    (501) staff       (20)       70 2023-09-20 13:49:45.000000 unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling/linear_gaussian/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)    64444 2024-03-13 15:10:50.000000 unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling/linear_gaussian/marginalizable_mixture_model.py
--rw-r--r--   0 michael    (501) staff       (20)    22466 2024-03-13 15:09:50.000000 unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling/linear_gaussian/marginalizable_state_space_model.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-13 15:16:52.466656 unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling/nonlinear/
--rw-r--r--   0 michael    (501) staff       (20)      321 2024-02-29 01:12:30.000000 unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling/nonlinear/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)      912 2024-03-13 15:12:37.000000 unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling/nonlinear/state_space_model.py
--rw-r--r--   0 michael    (501) staff       (20)     2880 2024-03-13 15:11:32.000000 unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling/nonlinear/state_space_model_classifier.py
--rw-r--r--   0 michael    (501) staff       (20)     5414 2024-03-13 15:11:40.000000 unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling/nonlinear/state_space_model_knn.py
--rw-r--r--   0 michael    (501) staff       (20)     4221 2024-03-13 15:11:55.000000 unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling/nonlinear/state_space_model_linear_gaussian.py
--rw-r--r--   0 michael    (501) staff       (20)     5544 2024-03-13 15:12:04.000000 unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling/nonlinear/state_space_model_linear_trans_knn_meas.py
--rw-r--r--   0 michael    (501) staff       (20)    17697 2024-03-13 15:12:27.000000 unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling/nonlinear/state_space_model_mixture.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-13 15:16:52.467515 unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling/util/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-09-20 13:49:49.000000 unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling/util/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     2472 2024-03-13 15:03:40.000000 unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling/util/util_post_hoc.py
--rw-r--r--   0 michael    (501) staff       (20)    35812 2024-03-13 15:03:28.000000 unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling/util/util_state_space.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-13 15:16:52.468384 unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     9296 2024-03-13 15:16:52.000000 unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)     1459 2024-03-13 15:16:52.000000 unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2024-03-13 15:16:52.000000 unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)      138 2024-03-13 15:16:52.000000 unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)       55 2024-03-13 15:16:52.000000 unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling.egg-info/top_level.txt
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-21 15:03:53.611456 unsupervised_multimodal_trajectory_modeling-2024.2.2/
+-rw-r--r--   0 michael    (501) staff       (20)     1084 2024-05-21 14:49:37.000000 unsupervised_multimodal_trajectory_modeling-2024.2.2/LICENSE.txt
+-rw-r--r--   0 michael    (501) staff       (20)     9393 2024-05-21 15:03:53.611226 unsupervised_multimodal_trajectory_modeling-2024.2.2/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     6926 2024-05-21 14:59:04.000000 unsupervised_multimodal_trajectory_modeling-2024.2.2/README.md
+-rw-r--r--   0 michael    (501) staff       (20)     1428 2024-05-21 15:01:54.000000 unsupervised_multimodal_trajectory_modeling-2024.2.2/pyproject.toml
+-rw-r--r--   0 michael    (501) staff       (20)       38 2024-05-21 15:03:53.611497 unsupervised_multimodal_trajectory_modeling-2024.2.2/setup.cfg
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-21 15:03:53.608238 unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2024-03-04 01:36:58.000000 unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling/__init__.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-21 15:03:53.609346 unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling/linear_gaussian/
+-rw-r--r--   0 michael    (501) staff       (20)       70 2023-09-20 13:49:45.000000 unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling/linear_gaussian/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)    64477 2024-05-21 14:56:24.000000 unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling/linear_gaussian/marginalizable_mixture_model.py
+-rw-r--r--   0 michael    (501) staff       (20)    22466 2024-05-21 14:56:24.000000 unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling/linear_gaussian/marginalizable_state_space_model.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-21 15:03:53.610387 unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling/nonlinear/
+-rw-r--r--   0 michael    (501) staff       (20)      321 2024-02-29 01:12:30.000000 unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling/nonlinear/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)      912 2024-03-13 15:12:37.000000 unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling/nonlinear/state_space_model.py
+-rw-r--r--   0 michael    (501) staff       (20)     2880 2024-03-13 15:11:32.000000 unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling/nonlinear/state_space_model_classifier.py
+-rw-r--r--   0 michael    (501) staff       (20)     5414 2024-03-13 15:11:40.000000 unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling/nonlinear/state_space_model_knn.py
+-rw-r--r--   0 michael    (501) staff       (20)     4221 2024-03-13 15:11:55.000000 unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling/nonlinear/state_space_model_linear_gaussian.py
+-rw-r--r--   0 michael    (501) staff       (20)     5544 2024-03-13 15:12:04.000000 unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling/nonlinear/state_space_model_linear_trans_knn_meas.py
+-rw-r--r--   0 michael    (501) staff       (20)    17697 2024-03-13 15:12:27.000000 unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling/nonlinear/state_space_model_mixture.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-21 15:03:53.610778 unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling/util/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-09-20 13:49:49.000000 unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling/util/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     2472 2024-05-21 14:56:24.000000 unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling/util/util_post_hoc.py
+-rw-r--r--   0 michael    (501) staff       (20)    35812 2024-05-21 14:56:24.000000 unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling/util/util_state_space.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-05-21 15:03:53.610995 unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     9393 2024-05-21 15:03:53.000000 unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     1459 2024-05-21 15:03:53.000000 unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2024-05-21 15:03:53.000000 unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)      138 2024-05-21 15:03:53.000000 unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)       49 2024-05-21 15:03:53.000000 unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling.egg-info/top_level.txt
```

### Comparing `unsupervised-multimodal-trajectory-modeling-2024.2.1/LICENSE.txt` & `unsupervised_multimodal_trajectory_modeling-2024.2.2/LICENSE.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-(c) 2023-2024 Michael C. Burkhart
+Copyright (c) 2024 Michael C. Burkhart, et al.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `unsupervised-multimodal-trajectory-modeling-2024.2.1/PKG-INFO` & `unsupervised_multimodal_trajectory_modeling-2024.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: unsupervised-multimodal-trajectory-modeling
-Version: 2024.2.1
+Version: 2024.2.2
 Summary: trains mixtures of state space models with expectation maximization
 Author-email: "Michael C. Burkhart" <mcb93@cam.ac.uk>
 License: MIT License
         
-        (c) 2023-2024 Michael C. Burkhart
+        Copyright (c) 2024 Michael C. Burkhart, et al.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -20,14 +20,15 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
+        
 Project-URL: Homepage, https://pypi.org/project/unsupervised-multimodal-trajectory-modeling/
 Project-URL: Repository, https://github.com/burkh4rt/Unsupervised-Multimodal-Trajectory-Modeling
 Keywords: unsupervised clustering,trajectory clustering,mixture models,state space models,machine learning
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -48,15 +49,15 @@
 Requires-Dist: tabulate>=0.9
 
 # Unsupervised Multimodal Trajectory Modeling
 
 [![DOI](https://zenodo.org/badge/692068384.svg)](https://zenodo.org/badge/latestdoi/692068384)
 
 We propose and validate a mixture of state space models to perform unsupervised
-clustering of short trajectories. Within the state space framework, we let
+clustering of short trajectories[^1]. Within the state space framework, we let
 expensive-to-gather biomarkers correspond to hidden states and readily
 obtainable cognitive metrics correspond to measurements. Upon training with
 expectation maximization, we find that our clusters stratify persons according
 to clinical outcome. Furthermore, we can effectively predict on held-out
 trajectories using cognitive metrics alone. Our approach accommodates missing
 data through model marginalization and generalizes across research and clinical
 cohorts.
@@ -84,40 +85,34 @@
 standardising to the longest available trajectory in a dataset and appending
 `np.nan`'s to shorter trajectories.
 
 ### Model specification
 
 We adopt a mixture of state space models for the data:
 
-<img src="figure1.png" 
-    alt="plate notation for mixture of state space models" 
-    style="max-width:700px;width:100%">
-
-given explicitly by:
-
 $$
 p(z^i_{1:T}, x^i_{1:T})
 		= \sum_{c=1}^{n_c} \pi_{c} \delta_{ \\{c=c^i \\} }
     \bigg( p(z_1^i| c)  \prod_{t=2}^T p(z_t^i | z_{t-1}^i, c)
-    \prod_{t=1}^T p(x_t^i | z_t^i, c) \bigg)
+    \prod_{t=1}^T p(x_t^i | z_t^i, c) \bigg).
 $$
 
 Each individual $i$ is independently assigned to some cluster $c^i$ with
 probability $\pi_{c}$, and then conditional on this cluster assignment, their
 initial state $z_1^i$ is drawn according to $p(z_1^i| c)$, with each subsequent
 state $z_t^i, 2\leq t \leq T$ being drawn in turn using the cluster-specific
 _state model_ $p(z_t^i | z_{t-1}^i, c)$, depending on the previous state. At
 each point in time, we obtain an observation $x_t^i$ from the cluster-specific
 _measurement model_ $p(x_t^i | z_t^i, c)$, depending on the current state. In
 what follows, we assume both the state and measurement models are stationary
 for each cluster, i.e. they are independent of $t$. In particular, for a given
 individual, the relationship between the state and measurement should not
 change over time.
 
-In our main framework, inspired by the work of Chiappa and Barber[^1], we
+In our main framework, inspired by the work of Chiappa and Barber[^2], we
 additionally assume that the cluster-specific state initialisation is Gaussian,
 i.e. $p(z_1^i| c) = \eta_d(z_1^i; m_c, S_c)$, and the cluster-specific state
 and measurement models are linear Gaussian, i.e.
 $p(z_t^i | z_{t-1}^i, c) = \eta_d(z_t^i; z_{t-1}^iA_c, \Gamma_c)$ and
 $p(x_t^i
 | z_t^i, c) = \eta_\ell(x_t^i; z_t^iH_c, \Lambda_c)$, where
 $\eta_d(\cdot, \mu,
@@ -132,15 +127,15 @@
 		\eta_\ell(x_t^i; z_t^iH_c, \Lambda_c) \bigg).
 $$
 
 In particular, we assume that the variables we are modeling are continuous and
 changing over time. When we train a model like the above, we take a dataset
 $\mathcal{D}$ and an arbitrary set of cluster assignments $c^i$ (as these are
 also latent/ hidden from us) and iteratively perform M and E steps (from which
-EM[^2] gets its name):
+EM[^3] gets its name):
 
 - [**E**] Expectation step: given the current model, we assign each data
   instance $(z^i_{1:T}, x^i_{1:T})$ to the cluster to which it is mostly likely
   to belong under the current model
 - [**M**] Maximization step: given the current cluster assignments, we compute
   the sample-level cluster assignment probabilities (the $\pi_c$) and optimal
   cluster-specific parameters
@@ -173,22 +168,27 @@
    yields numerical instabilities. Adding a small bit of noise to discrete
    features may remediate numerical instability to some extent.
 
 Another assumption that is easy-to-violate is our stationarity assumption for
 the measurement model.
 
 [^1]:
-    S. Chiappa and D. Barber. _Dirichlet Mixtures of Bayesian Linear Gaussian
-    State-Space Models: a Variational Approach._ Tech. rep. 161. Max Planck
-    Institute for Biological Cybernetics, 2007.
+    M. Burkhart, L. Lee, D. Vaghari, A. Toh, E. Chong, C. Chen, P. Tiňo, and Z.
+    Kourtzi, _Unsupervised multimodal modeling of cognitive and brain health
+    trajectories for early dementia prediction,_ Sci. Rep. 14 (2024)
 
 [^2]:
-    A. Dempster, N. Laird, and D. B. Rubin. _Maximum Likelihood from  
+    S. Chiappa and D. Barber, _Dirichlet Mixtures of Bayesian Linear Gaussian
+    State-Space Models: a Variational Approach,_ Tech. rep. 161, Max Planck
+    Institute for Biological Cybernetics, 2007.
+
+[^3]:
+    A. Dempster, N. Laird, and D. Rubin. _Maximum Likelihood from  
     Incomplete Data via the EM Algorithm._ J. Roy. Stat. Soc. Ser. B (Stat.
-    Methodol.) 39.1 (1977), pp. 1–38.
+    Methodol.) 39 (1977).
 
 <!--
 rm dist/*
 isort --profile black .
 black .
 prettier --write --print-width 79 --prose-wrap always **/*.md
 python3 -m build
```

### Comparing `unsupervised-multimodal-trajectory-modeling-2024.2.1/README.md` & `unsupervised_multimodal_trajectory_modeling-2024.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Unsupervised Multimodal Trajectory Modeling
 
 [![DOI](https://zenodo.org/badge/692068384.svg)](https://zenodo.org/badge/latestdoi/692068384)
 
 We propose and validate a mixture of state space models to perform unsupervised
-clustering of short trajectories. Within the state space framework, we let
+clustering of short trajectories[^1]. Within the state space framework, we let
 expensive-to-gather biomarkers correspond to hidden states and readily
 obtainable cognitive metrics correspond to measurements. Upon training with
 expectation maximization, we find that our clusters stratify persons according
 to clinical outcome. Furthermore, we can effectively predict on held-out
 trajectories using cognitive metrics alone. Our approach accommodates missing
 data through model marginalization and generalizes across research and clinical
 cohorts.
@@ -35,40 +35,34 @@
 standardising to the longest available trajectory in a dataset and appending
 `np.nan`'s to shorter trajectories.
 
 ### Model specification
 
 We adopt a mixture of state space models for the data:
 
-<img src="figure1.png" 
-    alt="plate notation for mixture of state space models" 
-    style="max-width:700px;width:100%">
-
-given explicitly by:
-
 $$
 p(z^i_{1:T}, x^i_{1:T})
 		= \sum_{c=1}^{n_c} \pi_{c} \delta_{ \\{c=c^i \\} }
     \bigg( p(z_1^i| c)  \prod_{t=2}^T p(z_t^i | z_{t-1}^i, c)
-    \prod_{t=1}^T p(x_t^i | z_t^i, c) \bigg)
+    \prod_{t=1}^T p(x_t^i | z_t^i, c) \bigg).
 $$
 
 Each individual $i$ is independently assigned to some cluster $c^i$ with
 probability $\pi_{c}$, and then conditional on this cluster assignment, their
 initial state $z_1^i$ is drawn according to $p(z_1^i| c)$, with each subsequent
 state $z_t^i, 2\leq t \leq T$ being drawn in turn using the cluster-specific
 _state model_ $p(z_t^i | z_{t-1}^i, c)$, depending on the previous state. At
 each point in time, we obtain an observation $x_t^i$ from the cluster-specific
 _measurement model_ $p(x_t^i | z_t^i, c)$, depending on the current state. In
 what follows, we assume both the state and measurement models are stationary
 for each cluster, i.e. they are independent of $t$. In particular, for a given
 individual, the relationship between the state and measurement should not
 change over time.
 
-In our main framework, inspired by the work of Chiappa and Barber[^1], we
+In our main framework, inspired by the work of Chiappa and Barber[^2], we
 additionally assume that the cluster-specific state initialisation is Gaussian,
 i.e. $p(z_1^i| c) = \eta_d(z_1^i; m_c, S_c)$, and the cluster-specific state
 and measurement models are linear Gaussian, i.e.
 $p(z_t^i | z_{t-1}^i, c) = \eta_d(z_t^i; z_{t-1}^iA_c, \Gamma_c)$ and
 $p(x_t^i
 | z_t^i, c) = \eta_\ell(x_t^i; z_t^iH_c, \Lambda_c)$, where
 $\eta_d(\cdot, \mu,
@@ -83,15 +77,15 @@
 		\eta_\ell(x_t^i; z_t^iH_c, \Lambda_c) \bigg).
 $$
 
 In particular, we assume that the variables we are modeling are continuous and
 changing over time. When we train a model like the above, we take a dataset
 $\mathcal{D}$ and an arbitrary set of cluster assignments $c^i$ (as these are
 also latent/ hidden from us) and iteratively perform M and E steps (from which
-EM[^2] gets its name):
+EM[^3] gets its name):
 
 - [**E**] Expectation step: given the current model, we assign each data
   instance $(z^i_{1:T}, x^i_{1:T})$ to the cluster to which it is mostly likely
   to belong under the current model
 - [**M**] Maximization step: given the current cluster assignments, we compute
   the sample-level cluster assignment probabilities (the $\pi_c$) and optimal
   cluster-specific parameters
@@ -124,22 +118,27 @@
    yields numerical instabilities. Adding a small bit of noise to discrete
    features may remediate numerical instability to some extent.
 
 Another assumption that is easy-to-violate is our stationarity assumption for
 the measurement model.
 
 [^1]:
-    S. Chiappa and D. Barber. _Dirichlet Mixtures of Bayesian Linear Gaussian
-    State-Space Models: a Variational Approach._ Tech. rep. 161. Max Planck
-    Institute for Biological Cybernetics, 2007.
+    M. Burkhart, L. Lee, D. Vaghari, A. Toh, E. Chong, C. Chen, P. Tiňo, and Z.
+    Kourtzi, _Unsupervised multimodal modeling of cognitive and brain health
+    trajectories for early dementia prediction,_ Sci. Rep. 14 (2024)
 
 [^2]:
-    A. Dempster, N. Laird, and D. B. Rubin. _Maximum Likelihood from  
+    S. Chiappa and D. Barber, _Dirichlet Mixtures of Bayesian Linear Gaussian
+    State-Space Models: a Variational Approach,_ Tech. rep. 161, Max Planck
+    Institute for Biological Cybernetics, 2007.
+
+[^3]:
+    A. Dempster, N. Laird, and D. Rubin. _Maximum Likelihood from  
     Incomplete Data via the EM Algorithm._ J. Roy. Stat. Soc. Ser. B (Stat.
-    Methodol.) 39.1 (1977), pp. 1–38.
+    Methodol.) 39 (1977).
 
 <!--
 rm dist/*
 isort --profile black .
 black .
 prettier --write --print-width 79 --prose-wrap always **/*.md
 python3 -m build
```

### Comparing `unsupervised-multimodal-trajectory-modeling-2024.2.1/pyproject.toml` & `unsupervised_multimodal_trajectory_modeling-2024.2.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -29,29 +29,32 @@
   "Development Status :: 2 - Pre-Alpha",
   "Intended Audience :: Science/Research",
   "License :: OSI Approved :: MIT License",
   "Natural Language :: English",
   "Programming Language :: Python :: 3",
   "Topic :: Scientific/Engineering :: Artificial Intelligence"
 ]
-version = "2024.2.1"
+version = "2024.2.2"
 requires-python = ">=3.10"
 
 [project.urls]
 Homepage = "https://pypi.org/project/unsupervised-multimodal-trajectory-modeling/"
 Repository = "https://github.com/burkh4rt/Unsupervised-Multimodal-Trajectory-Modeling"
 
 [tool.isort]
 profile = "black"
 
 [tool.setuptools.packages]
 find = {}
 
 [build-system]
-requires = ["setuptools>=69.0"]
+requires = [
+  "setuptools>=69.0",
+  "numpy>=1.26"
+]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 79
 target-version = [
   "py310",
   "py311"
```

### Comparing `unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling/linear_gaussian/marginalizable_mixture_model.py` & `unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling/linear_gaussian/marginalizable_mixture_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -613,16 +613,18 @@
                 for c in range(self.n_clusters)
             ]
         )
 
         return np.sum(
             np.log(self.cluster_propensities[cluster_assignment])
         ) + np.sum(
-            conditional_log_likelihoods[i, cluster_assignment[i]]
-            for i in range(cluster_assignment.size)
+            [
+                conditional_log_likelihoods[i, cluster_assignment[i]]
+                for i in range(cluster_assignment.size)
+            ]
         )
 
     def model_log_likelihood(
         self,
         *,
         states: np.array = None,
         observations: np.array = None,
@@ -1326,15 +1328,15 @@
         if (
             np.min(
                 np.bincount(self.cluster_assignment, minlength=self.n_clusters)
             )
             <= 3
         ):
             if verbose:
-                print(f"Encountered near-empty cluster.")
+                print("Encountered near-empty cluster.")
             return self
         self.M_step()
         if verbose:
             print(np.round(self.e_complete_data_log_lik(), 3))
         for i in range(n_steps):
             n_switches = self.E_step()
             if n_switches == 0:
@@ -1346,15 +1348,15 @@
                     np.bincount(
                         self.cluster_assignment, minlength=self.n_clusters
                     )
                 )
                 <= 3
             ):
                 if verbose:
-                    print(f"Encountered near-empty cluster.")
+                    print("Encountered near-empty cluster.")
                 break
             self.M_step()
             if verbose:
                 print(np.round(self.e_complete_data_log_lik(), 3))
         self.last_trained = (
             datetime.datetime.now(datetime.timezone.utc)
             .replace(microsecond=0)
@@ -1366,15 +1368,15 @@
     def train_with_multiple_random_starts(
         self,
         *,
         n_starts: int = 10,
         verbose: bool = False,
         n_steps: int = 100,
         return_objectives: bool = False,
-        use_cache: bool = False,
+        use_cache: bool = True,
     ):
         """train n_starts models from random initialisations
 
         Parameters
         ----------
         n_starts: int
             number of random initialisations to try
```

### Comparing `unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling/linear_gaussian/marginalizable_state_space_model.py` & `unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling/linear_gaussian/marginalizable_state_space_model.py`

 * *Files identical despite different names*

### Comparing `unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling/nonlinear/state_space_model.py` & `unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling/nonlinear/state_space_model.py`

 * *Files identical despite different names*

### Comparing `unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling/nonlinear/state_space_model_classifier.py` & `unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling/nonlinear/state_space_model_classifier.py`

 * *Files identical despite different names*

### Comparing `unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling/nonlinear/state_space_model_knn.py` & `unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling/nonlinear/state_space_model_knn.py`

 * *Files identical despite different names*

### Comparing `unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling/nonlinear/state_space_model_linear_gaussian.py` & `unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling/nonlinear/state_space_model_linear_gaussian.py`

 * *Files identical despite different names*

### Comparing `unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling/nonlinear/state_space_model_linear_trans_knn_meas.py` & `unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling/nonlinear/state_space_model_linear_trans_knn_meas.py`

 * *Files identical despite different names*

### Comparing `unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling/nonlinear/state_space_model_mixture.py` & `unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling/nonlinear/state_space_model_mixture.py`

 * *Files identical despite different names*

### Comparing `unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling/util/util_post_hoc.py` & `unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling/util/util_post_hoc.py`

 * *Files identical despite different names*

### Comparing `unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling/util/util_state_space.py` & `unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling/util/util_state_space.py`

 * *Files identical despite different names*

### Comparing `unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling.egg-info/PKG-INFO` & `unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: unsupervised-multimodal-trajectory-modeling
-Version: 2024.2.1
+Version: 2024.2.2
 Summary: trains mixtures of state space models with expectation maximization
 Author-email: "Michael C. Burkhart" <mcb93@cam.ac.uk>
 License: MIT License
         
-        (c) 2023-2024 Michael C. Burkhart
+        Copyright (c) 2024 Michael C. Burkhart, et al.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -20,14 +20,15 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
+        
 Project-URL: Homepage, https://pypi.org/project/unsupervised-multimodal-trajectory-modeling/
 Project-URL: Repository, https://github.com/burkh4rt/Unsupervised-Multimodal-Trajectory-Modeling
 Keywords: unsupervised clustering,trajectory clustering,mixture models,state space models,machine learning
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -48,15 +49,15 @@
 Requires-Dist: tabulate>=0.9
 
 # Unsupervised Multimodal Trajectory Modeling
 
 [![DOI](https://zenodo.org/badge/692068384.svg)](https://zenodo.org/badge/latestdoi/692068384)
 
 We propose and validate a mixture of state space models to perform unsupervised
-clustering of short trajectories. Within the state space framework, we let
+clustering of short trajectories[^1]. Within the state space framework, we let
 expensive-to-gather biomarkers correspond to hidden states and readily
 obtainable cognitive metrics correspond to measurements. Upon training with
 expectation maximization, we find that our clusters stratify persons according
 to clinical outcome. Furthermore, we can effectively predict on held-out
 trajectories using cognitive metrics alone. Our approach accommodates missing
 data through model marginalization and generalizes across research and clinical
 cohorts.
@@ -84,40 +85,34 @@
 standardising to the longest available trajectory in a dataset and appending
 `np.nan`'s to shorter trajectories.
 
 ### Model specification
 
 We adopt a mixture of state space models for the data:
 
-<img src="figure1.png" 
-    alt="plate notation for mixture of state space models" 
-    style="max-width:700px;width:100%">
-
-given explicitly by:
-
 $$
 p(z^i_{1:T}, x^i_{1:T})
 		= \sum_{c=1}^{n_c} \pi_{c} \delta_{ \\{c=c^i \\} }
     \bigg( p(z_1^i| c)  \prod_{t=2}^T p(z_t^i | z_{t-1}^i, c)
-    \prod_{t=1}^T p(x_t^i | z_t^i, c) \bigg)
+    \prod_{t=1}^T p(x_t^i | z_t^i, c) \bigg).
 $$
 
 Each individual $i$ is independently assigned to some cluster $c^i$ with
 probability $\pi_{c}$, and then conditional on this cluster assignment, their
 initial state $z_1^i$ is drawn according to $p(z_1^i| c)$, with each subsequent
 state $z_t^i, 2\leq t \leq T$ being drawn in turn using the cluster-specific
 _state model_ $p(z_t^i | z_{t-1}^i, c)$, depending on the previous state. At
 each point in time, we obtain an observation $x_t^i$ from the cluster-specific
 _measurement model_ $p(x_t^i | z_t^i, c)$, depending on the current state. In
 what follows, we assume both the state and measurement models are stationary
 for each cluster, i.e. they are independent of $t$. In particular, for a given
 individual, the relationship between the state and measurement should not
 change over time.
 
-In our main framework, inspired by the work of Chiappa and Barber[^1], we
+In our main framework, inspired by the work of Chiappa and Barber[^2], we
 additionally assume that the cluster-specific state initialisation is Gaussian,
 i.e. $p(z_1^i| c) = \eta_d(z_1^i; m_c, S_c)$, and the cluster-specific state
 and measurement models are linear Gaussian, i.e.
 $p(z_t^i | z_{t-1}^i, c) = \eta_d(z_t^i; z_{t-1}^iA_c, \Gamma_c)$ and
 $p(x_t^i
 | z_t^i, c) = \eta_\ell(x_t^i; z_t^iH_c, \Lambda_c)$, where
 $\eta_d(\cdot, \mu,
@@ -132,15 +127,15 @@
 		\eta_\ell(x_t^i; z_t^iH_c, \Lambda_c) \bigg).
 $$
 
 In particular, we assume that the variables we are modeling are continuous and
 changing over time. When we train a model like the above, we take a dataset
 $\mathcal{D}$ and an arbitrary set of cluster assignments $c^i$ (as these are
 also latent/ hidden from us) and iteratively perform M and E steps (from which
-EM[^2] gets its name):
+EM[^3] gets its name):
 
 - [**E**] Expectation step: given the current model, we assign each data
   instance $(z^i_{1:T}, x^i_{1:T})$ to the cluster to which it is mostly likely
   to belong under the current model
 - [**M**] Maximization step: given the current cluster assignments, we compute
   the sample-level cluster assignment probabilities (the $\pi_c$) and optimal
   cluster-specific parameters
@@ -173,22 +168,27 @@
    yields numerical instabilities. Adding a small bit of noise to discrete
    features may remediate numerical instability to some extent.
 
 Another assumption that is easy-to-violate is our stationarity assumption for
 the measurement model.
 
 [^1]:
-    S. Chiappa and D. Barber. _Dirichlet Mixtures of Bayesian Linear Gaussian
-    State-Space Models: a Variational Approach._ Tech. rep. 161. Max Planck
-    Institute for Biological Cybernetics, 2007.
+    M. Burkhart, L. Lee, D. Vaghari, A. Toh, E. Chong, C. Chen, P. Tiňo, and Z.
+    Kourtzi, _Unsupervised multimodal modeling of cognitive and brain health
+    trajectories for early dementia prediction,_ Sci. Rep. 14 (2024)
 
 [^2]:
-    A. Dempster, N. Laird, and D. B. Rubin. _Maximum Likelihood from  
+    S. Chiappa and D. Barber, _Dirichlet Mixtures of Bayesian Linear Gaussian
+    State-Space Models: a Variational Approach,_ Tech. rep. 161, Max Planck
+    Institute for Biological Cybernetics, 2007.
+
+[^3]:
+    A. Dempster, N. Laird, and D. Rubin. _Maximum Likelihood from  
     Incomplete Data via the EM Algorithm._ J. Roy. Stat. Soc. Ser. B (Stat.
-    Methodol.) 39.1 (1977), pp. 1–38.
+    Methodol.) 39 (1977).
 
 <!--
 rm dist/*
 isort --profile black .
 black .
 prettier --write --print-width 79 --prose-wrap always **/*.md
 python3 -m build
```

### Comparing `unsupervised-multimodal-trajectory-modeling-2024.2.1/unsupervised_multimodal_trajectory_modeling.egg-info/SOURCES.txt` & `unsupervised_multimodal_trajectory_modeling-2024.2.2/unsupervised_multimodal_trajectory_modeling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

