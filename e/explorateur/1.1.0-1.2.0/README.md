# Comparing `tmp/explorateur-1.1.0.tar.gz` & `tmp/explorateur-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "explorateur-1.1.0.tar", last modified: Wed May 15 02:12:45 2024, max compression
+gzip compressed data, was "explorateur-1.2.0.tar", last modified: Tue May 21 06:10:36 2024, max compression
```

## Comparing `explorateur-1.1.0.tar` & `explorateur-1.2.0.tar`

### file list

```diff
@@ -1,48 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 02:12:45.062038 explorateur-1.1.0/
--rw-rw-rw-   0        0        0    11544 2024-05-14 08:36:47.000000 explorateur-1.1.0/LICENSE.md
--rw-rw-rw-   0        0        0       20 2024-03-11 23:23:44.000000 explorateur-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0    11256 2024-05-15 02:12:45.062038 explorateur-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    10799 2024-05-15 02:07:24.000000 explorateur-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 02:12:45.002572 explorateur-1.1.0/explorateur/
--rw-rw-rw-   0        0        0      277 2024-05-14 08:36:47.000000 explorateur-1.1.0/explorateur/__init__.py
--rw-rw-rw-   0        0        0       23 2024-05-15 02:10:56.000000 explorateur-1.1.0/explorateur/_version.py
--rw-rw-rw-   0        0        0    21032 2024-05-15 01:41:00.000000 explorateur-1.1.0/explorateur/explorateur.py
-drwxrwxrwx   0        0        0        0 2024-05-15 02:12:45.038335 explorateur-1.1.0/explorateur/search/
--rw-rw-rw-   0        0        0        0 2024-03-11 23:23:44.000000 explorateur-1.1.0/explorateur/search/__init__.py
--rw-rw-rw-   0        0        0      724 2024-05-14 08:36:47.000000 explorateur-1.1.0/explorateur/search/decision.py
--rw-rw-rw-   0        0        0      380 2024-05-14 08:36:47.000000 explorateur-1.1.0/explorateur/search/exploration_type.py
--rw-rw-rw-   0        0        0      169 2024-05-14 08:36:47.000000 explorateur-1.1.0/explorateur/search/search_type.py
--rw-rw-rw-   0        0        0      210 2024-05-14 08:36:47.000000 explorateur-1.1.0/explorateur/search/storage.py
--rw-rw-rw-   0        0        0      361 2024-05-14 08:36:47.000000 explorateur-1.1.0/explorateur/search/transition.py
-drwxrwxrwx   0        0        0        0 2024-05-15 02:12:45.041419 explorateur-1.1.0/explorateur/state/
--rw-rw-rw-   0        0        0        0 2024-03-11 23:23:44.000000 explorateur-1.1.0/explorateur/state/__init__.py
--rw-rw-rw-   0        0        0      847 2024-05-14 08:36:47.000000 explorateur-1.1.0/explorateur/state/base_move.py
--rw-rw-rw-   0        0        0     2797 2024-05-14 08:36:47.000000 explorateur-1.1.0/explorateur/state/base_state.py
-drwxrwxrwx   0        0        0        0 2024-05-15 02:12:45.049850 explorateur-1.1.0/explorateur/state/storage/
--rw-rw-rw-   0        0        0        0 2024-03-11 23:23:44.000000 explorateur-1.1.0/explorateur/state/storage/__init__.py
--rw-rw-rw-   0        0        0      943 2024-05-14 08:36:47.000000 explorateur-1.1.0/explorateur/state/storage/base_storage.py
--rw-rw-rw-   0        0        0     1458 2024-05-14 08:36:47.000000 explorateur-1.1.0/explorateur/state/storage/factory.py
--rw-rw-rw-   0        0        0      821 2024-05-14 08:36:47.000000 explorateur-1.1.0/explorateur/state/storage/hash.py
--rw-rw-rw-   0        0        0     1103 2024-05-14 08:36:47.000000 explorateur-1.1.0/explorateur/state/storage/priority_queue.py
--rw-rw-rw-   0        0        0      923 2024-05-14 08:36:47.000000 explorateur-1.1.0/explorateur/state/storage/queue.py
--rw-rw-rw-   0        0        0      922 2024-05-14 08:36:47.000000 explorateur-1.1.0/explorateur/state/storage/stack.py
--rw-rw-rw-   0        0        0     1796 2024-05-15 00:33:30.000000 explorateur-1.1.0/explorateur/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-15 02:12:45.031445 explorateur-1.1.0/explorateur.egg-info/
--rw-rw-rw-   0        0        0    11256 2024-05-15 02:12:44.000000 explorateur-1.1.0/explorateur.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1143 2024-05-15 02:12:44.000000 explorateur-1.1.0/explorateur.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 02:12:44.000000 explorateur-1.1.0/explorateur.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-15 02:12:44.000000 explorateur-1.1.0/explorateur.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 02:12:45.063088 explorateur-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1078 2024-05-14 08:36:47.000000 explorateur-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 02:12:45.061023 explorateur-1.1.0/tests/
--rw-rw-rw-   0        0        0     6129 2024-05-15 01:34:14.000000 explorateur-1.1.0/tests/test_base.py
--rw-rw-rw-   0        0        0     1677 2024-05-15 01:23:49.000000 explorateur-1.1.0/tests/test_graph_best_first.py
--rw-rw-rw-   0        0        0     3121 2024-05-15 01:45:08.000000 explorateur-1.1.0/tests/test_graph_breadth_first.py
--rw-rw-rw-   0        0        0     1611 2024-05-15 01:42:39.000000 explorateur-1.1.0/tests/test_graph_depth_first.py
--rw-rw-rw-   0        0        0     4507 2024-05-15 00:59:17.000000 explorateur-1.1.0/tests/test_invalid.py
--rw-rw-rw-   0        0        0     2863 2024-05-15 01:41:24.000000 explorateur-1.1.0/tests/test_stop_criteria.py
--rw-rw-rw-   0        0        0     1615 2024-05-14 23:00:28.000000 explorateur-1.1.0/tests/test_storage.py
--rw-rw-rw-   0        0        0     1674 2024-05-15 01:23:18.000000 explorateur-1.1.0/tests/test_tree_best_first.py
--rw-rw-rw-   0        0        0     3116 2024-05-15 01:44:08.000000 explorateur-1.1.0/tests/test_tree_breadth_first.py
--rw-rw-rw-   0        0        0     3130 2024-05-15 01:40:27.000000 explorateur-1.1.0/tests/test_tree_depth_first.py
--rw-rw-rw-   0        0        0     1073 2024-05-15 00:38:28.000000 explorateur-1.1.0/tests/test_usage_example.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:10:36.638381 explorateur-1.2.0/
+-rw-rw-rw-   0        0        0    11544 2024-05-14 08:36:47.000000 explorateur-1.2.0/LICENSE.md
+-rw-rw-rw-   0        0        0    11728 2024-05-21 06:10:36.637391 explorateur-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11271 2024-05-17 02:26:20.000000 explorateur-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 06:10:36.380041 explorateur-1.2.0/explorateur/
+-rw-rw-rw-   0        0        0      319 2024-05-16 07:18:34.000000 explorateur-1.2.0/explorateur/__init__.py
+-rw-rw-rw-   0        0        0       23 2024-05-21 06:09:47.000000 explorateur-1.2.0/explorateur/_version.py
+-rw-rw-rw-   0        0        0    21033 2024-05-21 06:05:06.000000 explorateur-1.2.0/explorateur/explorateur.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:10:36.495059 explorateur-1.2.0/explorateur/search/
+-rw-rw-rw-   0        0        0        0 2024-03-11 23:23:44.000000 explorateur-1.2.0/explorateur/search/__init__.py
+-rw-rw-rw-   0        0        0      380 2024-05-14 08:36:47.000000 explorateur-1.2.0/explorateur/search/exploration_type.py
+-rw-rw-rw-   0        0        0      169 2024-05-14 08:36:47.000000 explorateur-1.2.0/explorateur/search/search_type.py
+-rw-rw-rw-   0        0        0      210 2024-05-14 08:36:47.000000 explorateur-1.2.0/explorateur/search/storage.py
+-rw-rw-rw-   0        0        0      361 2024-05-14 08:36:47.000000 explorateur-1.2.0/explorateur/search/transition.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:10:36.506736 explorateur-1.2.0/explorateur/state/
+-rw-rw-rw-   0        0        0        0 2024-03-11 23:23:44.000000 explorateur-1.2.0/explorateur/state/__init__.py
+-rw-rw-rw-   0        0        0      847 2024-05-16 03:53:11.000000 explorateur-1.2.0/explorateur/state/base_move.py
+-rw-rw-rw-   0        0        0     2797 2024-05-21 05:48:23.000000 explorateur-1.2.0/explorateur/state/base_state.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:10:36.527592 explorateur-1.2.0/explorateur/state/storage/
+-rw-rw-rw-   0        0        0        0 2024-03-11 23:23:44.000000 explorateur-1.2.0/explorateur/state/storage/__init__.py
+-rw-rw-rw-   0        0        0      943 2024-05-21 05:35:24.000000 explorateur-1.2.0/explorateur/state/storage/base_storage.py
+-rw-rw-rw-   0        0        0     1458 2024-05-14 08:36:47.000000 explorateur-1.2.0/explorateur/state/storage/factory.py
+-rw-rw-rw-   0        0        0      813 2024-05-21 05:36:07.000000 explorateur-1.2.0/explorateur/state/storage/hash.py
+-rw-rw-rw-   0        0        0     1089 2024-05-21 05:36:07.000000 explorateur-1.2.0/explorateur/state/storage/priority_queue.py
+-rw-rw-rw-   0        0        0      918 2024-05-21 05:36:18.000000 explorateur-1.2.0/explorateur/state/storage/queue.py
+-rw-rw-rw-   0        0        0      917 2024-05-21 05:36:37.000000 explorateur-1.2.0/explorateur/state/storage/stack.py
+-rw-rw-rw-   0        0        0     4181 2024-05-21 05:35:24.000000 explorateur-1.2.0/explorateur/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:10:36.434249 explorateur-1.2.0/explorateur.egg-info/
+-rw-rw-rw-   0        0        0    11728 2024-05-21 06:10:35.000000 explorateur-1.2.0/explorateur.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1100 2024-05-21 06:10:36.000000 explorateur-1.2.0/explorateur.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 06:10:35.000000 explorateur-1.2.0/explorateur.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-21 06:10:35.000000 explorateur-1.2.0/explorateur.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 06:10:36.638381 explorateur-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1078 2024-05-14 08:36:47.000000 explorateur-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:10:36.633374 explorateur-1.2.0/tests/
+-rw-rw-rw-   0        0        0     6654 2024-05-21 05:48:23.000000 explorateur-1.2.0/tests/test_base.py
+-rw-rw-rw-   0        0        0     1677 2024-05-15 01:23:49.000000 explorateur-1.2.0/tests/test_graph_best_first.py
+-rw-rw-rw-   0        0        0     3197 2024-05-16 06:45:04.000000 explorateur-1.2.0/tests/test_graph_breadth_first.py
+-rw-rw-rw-   0        0        0     1674 2024-05-21 05:58:12.000000 explorateur-1.2.0/tests/test_graph_depth_first.py
+-rw-rw-rw-   0        0        0     4507 2024-05-15 00:59:17.000000 explorateur-1.2.0/tests/test_invalid.py
+-rw-rw-rw-   0        0        0     3926 2024-05-21 06:05:20.000000 explorateur-1.2.0/tests/test_stop_criteria.py
+-rw-rw-rw-   0        0        0     2503 2024-05-21 05:57:19.000000 explorateur-1.2.0/tests/test_storage.py
+-rw-rw-rw-   0        0        0     1674 2024-05-15 01:23:18.000000 explorateur-1.2.0/tests/test_tree_best_first.py
+-rw-rw-rw-   0        0        0     3151 2024-05-21 03:06:07.000000 explorateur-1.2.0/tests/test_tree_breadth_first.py
+-rw-rw-rw-   0        0        0     3205 2024-05-21 05:49:48.000000 explorateur-1.2.0/tests/test_tree_depth_first.py
+-rw-rw-rw-   0        0        0     1130 2024-05-16 02:36:40.000000 explorateur-1.2.0/tests/test_usage_example.py
```

### Comparing `explorateur-1.1.0/LICENSE.md` & `explorateur-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `explorateur-1.1.0/PKG-INFO` & `explorateur-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,8 @@
-Metadata-Version: 2.1
-Name: explorateur
-Version: 1.1.0
-Summary: State space search
-Home-page: https://github.com/skadio/explorateur
-Author: xxx
-Project-URL: Documentation, https://xxx
-Project-URL: Source, https://xxx
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
+[![PyPI version fury.io](https://badge.fury.io/py/explorateur.svg)](https://pypi.python.org/pypi/explorateur/) [![PyPI license](https://img.shields.io/pypi/l/explorateur.svg)](https://pypi.python.org/pypi/explorateur/) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com) [![Downloads](https://static.pepy.tech/personalized-badge/explorateur?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/explorateur)
 
 # Explorateur
 
 Explorateur is a Python library to conduct [State-Space-Search (SSS)](https://en.wikipedia.org/wiki/State_space_search), a powerful framework for solving problems that require search over a collection of states. 
 
 Explorateur performs **generic state-space-search** over **problem-specific states and moves**. The user defines the `BaseState` and `BaseMove` and the library drives the search for solutions.
 
@@ -33,29 +21,29 @@
 ### Exploration Strategy 
 - `BreadthFirst` in uninformed fashion 
 - `DepthFirst` in uninformed fashion
 - `BestFirst` in informed fashion assuming an objective function evaluates the solution quality of a state.
 
 ## Quick Start
 
-To use Explorateur, you need to define `BaseState` and `BaseMove`, with the quick start template below.  
+To use Explorateur, you need to define `BaseState` and `BaseMove` as in the template below.  
 
 ```python
 from explorateur import Explorateur, BaseMove, BaseState, ExplorationType, SearchType
 
 
 # TODO Implement your own Search Moves
 class MyMove(BaseMove):
 
     def __init__(self):
         # TODO Your move object
         pass
 
     def __str__(self) -> str:
-        # TODO Your mvoe string, also used for node labels in DOT graph
+        # TODO Your move string, also used for node labels in DOT graph
         pass
 
 
 # TODO Implement your own Search State 
 class MyState(BaseState):
 
     def __init__(self):
@@ -74,15 +62,15 @@
         # TODO Execute the move on the state and return success flag
         pass
 
     def __str__(self) -> str:
         # TODO Your state string, also used for node labels in DOT graph
         pass
 
-# Explorateur
+# Explarateur
 explorer = Explorateur()
 
 # Initial state
 initial_state = MyState()
 
 # Search for solutions
 if explorer.search(initial_state,
@@ -103,15 +91,15 @@
 print("Total Decisions:", explorer.num_decisions)
 print("Total Failures:", explorer.num_failed_decisions)
 print("Total Time:", explorer.total_time)
 ```
 
 ## Concrete Example
 
-Here is a concrete implementation to solve a toy [Constraint Satisfaction Problem](examples/usage_example.py) with the corresponding [search dot graph](examples/usage_example.dot)  and [search visualization](https://dreampuf.github.io/GraphvizOnline/#digraph%20G%20%7B%0D%0Aspline%3Dline%3B%0D%0A%22State%20ID%3A%200%0D%0AAssignment%3A%20%7B%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%2C%202%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%201%0D%0AAssignment%3A%20%7B'x'%3A%201%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22x%20%3D%3D%201%22%5D%3B%0D%0A%22State%20ID%3A%201%0D%0AAssignment%3A%20%7B'x'%3A%201%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%202%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22y%20%3D%3D%2010%22%5D%3B%0D%0A%22State%20ID%3A%202%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%203%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2010%2C%20'z'%3A%20100%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%5D%7D%22%20%5Blabel%3D%22z%20%3D%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%202%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%204%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2010%2C%20'z'%3A%20200%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B200%5D%7D%22%20%5Blabel%3D%22z%20!%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%201%0D%0AAssignment%3A%20%7B'x'%3A%201%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%205%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22y%20!%3D%2010%22%5D%3B%0D%0A%22State%20ID%3A%205%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%206%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2020%2C%20'z'%3A%20100%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%5D%7D%22%20%5Blabel%3D%22z%20%3D%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%205%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%207%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2020%2C%20'z'%3A%20200%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B200%5D%7D%22%20%5Blabel%3D%22z%20!%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%200%0D%0AAssignment%3A%20%7B%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%2C%202%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%208%0D%0AAssignment%3A%20%7B'x'%3A%202%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22x%20!%3D%201%22%5D%3B%0D%0A%22State%20ID%3A%208%0D%0AAssignment%3A%20%7B'x'%3A%202%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%209%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22y%20%3D%3D%2010%22%5D%3B%0D%0A%22State%20ID%3A%209%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%2010%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2010%2C%20'z'%3A%20100%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%5D%7D%22%20%5Blabel%3D%22z%20%3D%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%209%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%2011%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2010%2C%20'z'%3A%20200%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B200%5D%7D%22%20%5Blabel%3D%22z%20!%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%208%0D%0AAssignment%3A%20%7B'x'%3A%202%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%2012%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22y%20!%3D%2010%22%5D%3B%0D%0A%22State%20ID%3A%2012%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%2013%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2020%2C%20'z'%3A%20100%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%5D%7D%22%20%5Blabel%3D%22z%20%3D%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%2012%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%2014%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2020%2C%20'z'%3A%20200%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B200%5D%7D%22%20%5Blabel%3D%22z%20!%3D%20100%22%5D%3B%0D%0A%7D).
+Here is a concrete implementation to solve a toy [Constraint Satisfaction Problem](examples/backtrack_tree_search/main.py) using backtracking tree search, with the corresponding [search dot graph](examples/backtrack_tree_search/output.dot)  and [search visualization](https://dreampuf.github.io/GraphvizOnline/#digraph%20G%20%7B%0D%0Aspline%3Dline%3B%0D%0A%22State%20ID%3A%200%0D%0AAssignment%3A%20%7B%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%2C%202%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%201%0D%0AAssignment%3A%20%7B'x'%3A%201%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22x%20%3D%3D%201%22%5D%3B%0D%0A%22State%20ID%3A%201%0D%0AAssignment%3A%20%7B'x'%3A%201%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%202%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22y%20%3D%3D%2010%22%5D%3B%0D%0A%22State%20ID%3A%202%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%203%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2010%2C%20'z'%3A%20100%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%5D%7D%22%20%5Blabel%3D%22z%20%3D%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%202%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%204%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2010%2C%20'z'%3A%20200%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B200%5D%7D%22%20%5Blabel%3D%22z%20!%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%201%0D%0AAssignment%3A%20%7B'x'%3A%201%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%205%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22y%20!%3D%2010%22%5D%3B%0D%0A%22State%20ID%3A%205%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%206%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2020%2C%20'z'%3A%20100%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%5D%7D%22%20%5Blabel%3D%22z%20%3D%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%205%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%207%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2020%2C%20'z'%3A%20200%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B200%5D%7D%22%20%5Blabel%3D%22z%20!%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%200%0D%0AAssignment%3A%20%7B%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%2C%202%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%208%0D%0AAssignment%3A%20%7B'x'%3A%202%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22x%20!%3D%201%22%5D%3B%0D%0A%22State%20ID%3A%208%0D%0AAssignment%3A%20%7B'x'%3A%202%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%209%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22y%20%3D%3D%2010%22%5D%3B%0D%0A%22State%20ID%3A%209%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%2010%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2010%2C%20'z'%3A%20100%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%5D%7D%22%20%5Blabel%3D%22z%20%3D%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%209%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%2011%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2010%2C%20'z'%3A%20200%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B200%5D%7D%22%20%5Blabel%3D%22z%20!%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%208%0D%0AAssignment%3A%20%7B'x'%3A%202%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%2012%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22y%20!%3D%2010%22%5D%3B%0D%0A%22State%20ID%3A%2012%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%2013%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2020%2C%20'z'%3A%20100%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%5D%7D%22%20%5Blabel%3D%22z%20%3D%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%2012%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%2014%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2020%2C%20'z'%3A%20200%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B200%5D%7D%22%20%5Blabel%3D%22z%20!%3D%20100%22%5D%3B%0D%0A%7D).
 
 
 ## Install from PyPI
 
 Explorateur can be installed from PyPI using `pip install explorateur`
 
 ## Install from Source
@@ -147,20 +135,14 @@
 To confirm that installation was successful, try importing Explorateur after `pip install explorateur`
 
 ```
 import explorateur
 print(explorateur.__version__)
 ```
 
-## Changelog
-
-| Date         | Notes           |
-|--------------|-----------------|
-| 15 May, 2024 | Initial release |
-
 ## Support
 
 Please submit bug reports and feature requests as [Issues](https://github.com/explorateur/issues).
 
 ## License
 
 Explorateur is licensed under the [Apache License 2.0](LICENSE.md).
```

### Comparing `explorateur-1.1.0/README.md` & `explorateur-1.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: explorateur
+Version: 1.2.0
+Summary: State space search
+Home-page: https://github.com/skadio/explorateur
+Author: xxx
+Project-URL: Documentation, https://xxx
+Project-URL: Source, https://xxx
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+[![PyPI version fury.io](https://badge.fury.io/py/explorateur.svg)](https://pypi.python.org/pypi/explorateur/) [![PyPI license](https://img.shields.io/pypi/l/explorateur.svg)](https://pypi.python.org/pypi/explorateur/) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com) [![Downloads](https://static.pepy.tech/personalized-badge/explorateur?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/explorateur)
+
 # Explorateur
 
 Explorateur is a Python library to conduct [State-Space-Search (SSS)](https://en.wikipedia.org/wiki/State_space_search), a powerful framework for solving problems that require search over a collection of states. 
 
 Explorateur performs **generic state-space-search** over **problem-specific states and moves**. The user defines the `BaseState` and `BaseMove` and the library drives the search for solutions.
 
 Given an initial user state, Explorateur performs iterative search moves until a stopping condition is reached: 
@@ -19,29 +35,29 @@
 ### Exploration Strategy 
 - `BreadthFirst` in uninformed fashion 
 - `DepthFirst` in uninformed fashion
 - `BestFirst` in informed fashion assuming an objective function evaluates the solution quality of a state.
 
 ## Quick Start
 
-To use Explorateur, you need to define `BaseState` and `BaseMove`, with the quick start template below.  
+To use Explorateur, you need to define `BaseState` and `BaseMove` as in the template below.  
 
 ```python
 from explorateur import Explorateur, BaseMove, BaseState, ExplorationType, SearchType
 
 
 # TODO Implement your own Search Moves
 class MyMove(BaseMove):
 
     def __init__(self):
         # TODO Your move object
         pass
 
     def __str__(self) -> str:
-        # TODO Your mvoe string, also used for node labels in DOT graph
+        # TODO Your move string, also used for node labels in DOT graph
         pass
 
 
 # TODO Implement your own Search State 
 class MyState(BaseState):
 
     def __init__(self):
@@ -60,15 +76,15 @@
         # TODO Execute the move on the state and return success flag
         pass
 
     def __str__(self) -> str:
         # TODO Your state string, also used for node labels in DOT graph
         pass
 
-# Explorateur
+# Explarateur
 explorer = Explorateur()
 
 # Initial state
 initial_state = MyState()
 
 # Search for solutions
 if explorer.search(initial_state,
@@ -89,15 +105,15 @@
 print("Total Decisions:", explorer.num_decisions)
 print("Total Failures:", explorer.num_failed_decisions)
 print("Total Time:", explorer.total_time)
 ```
 
 ## Concrete Example
 
-Here is a concrete implementation to solve a toy [Constraint Satisfaction Problem](examples/usage_example.py) with the corresponding [search dot graph](examples/usage_example.dot)  and [search visualization](https://dreampuf.github.io/GraphvizOnline/#digraph%20G%20%7B%0D%0Aspline%3Dline%3B%0D%0A%22State%20ID%3A%200%0D%0AAssignment%3A%20%7B%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%2C%202%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%201%0D%0AAssignment%3A%20%7B'x'%3A%201%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22x%20%3D%3D%201%22%5D%3B%0D%0A%22State%20ID%3A%201%0D%0AAssignment%3A%20%7B'x'%3A%201%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%202%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22y%20%3D%3D%2010%22%5D%3B%0D%0A%22State%20ID%3A%202%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%203%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2010%2C%20'z'%3A%20100%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%5D%7D%22%20%5Blabel%3D%22z%20%3D%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%202%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%204%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2010%2C%20'z'%3A%20200%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B200%5D%7D%22%20%5Blabel%3D%22z%20!%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%201%0D%0AAssignment%3A%20%7B'x'%3A%201%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%205%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22y%20!%3D%2010%22%5D%3B%0D%0A%22State%20ID%3A%205%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%206%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2020%2C%20'z'%3A%20100%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%5D%7D%22%20%5Blabel%3D%22z%20%3D%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%205%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%207%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2020%2C%20'z'%3A%20200%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B200%5D%7D%22%20%5Blabel%3D%22z%20!%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%200%0D%0AAssignment%3A%20%7B%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%2C%202%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%208%0D%0AAssignment%3A%20%7B'x'%3A%202%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22x%20!%3D%201%22%5D%3B%0D%0A%22State%20ID%3A%208%0D%0AAssignment%3A%20%7B'x'%3A%202%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%209%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22y%20%3D%3D%2010%22%5D%3B%0D%0A%22State%20ID%3A%209%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%2010%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2010%2C%20'z'%3A%20100%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%5D%7D%22%20%5Blabel%3D%22z%20%3D%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%209%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%2011%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2010%2C%20'z'%3A%20200%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B200%5D%7D%22%20%5Blabel%3D%22z%20!%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%208%0D%0AAssignment%3A%20%7B'x'%3A%202%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%2012%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22y%20!%3D%2010%22%5D%3B%0D%0A%22State%20ID%3A%2012%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%2013%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2020%2C%20'z'%3A%20100%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%5D%7D%22%20%5Blabel%3D%22z%20%3D%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%2012%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%2014%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2020%2C%20'z'%3A%20200%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B200%5D%7D%22%20%5Blabel%3D%22z%20!%3D%20100%22%5D%3B%0D%0A%7D).
+Here is a concrete implementation to solve a toy [Constraint Satisfaction Problem](examples/backtrack_tree_search/main.py) using backtracking tree search, with the corresponding [search dot graph](examples/backtrack_tree_search/output.dot)  and [search visualization](https://dreampuf.github.io/GraphvizOnline/#digraph%20G%20%7B%0D%0Aspline%3Dline%3B%0D%0A%22State%20ID%3A%200%0D%0AAssignment%3A%20%7B%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%2C%202%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%201%0D%0AAssignment%3A%20%7B'x'%3A%201%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22x%20%3D%3D%201%22%5D%3B%0D%0A%22State%20ID%3A%201%0D%0AAssignment%3A%20%7B'x'%3A%201%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%202%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22y%20%3D%3D%2010%22%5D%3B%0D%0A%22State%20ID%3A%202%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%203%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2010%2C%20'z'%3A%20100%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%5D%7D%22%20%5Blabel%3D%22z%20%3D%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%202%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%204%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2010%2C%20'z'%3A%20200%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B200%5D%7D%22%20%5Blabel%3D%22z%20!%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%201%0D%0AAssignment%3A%20%7B'x'%3A%201%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%205%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22y%20!%3D%2010%22%5D%3B%0D%0A%22State%20ID%3A%205%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%206%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2020%2C%20'z'%3A%20100%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%5D%7D%22%20%5Blabel%3D%22z%20%3D%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%205%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%207%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2020%2C%20'z'%3A%20200%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B200%5D%7D%22%20%5Blabel%3D%22z%20!%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%200%0D%0AAssignment%3A%20%7B%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%2C%202%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%208%0D%0AAssignment%3A%20%7B'x'%3A%202%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22x%20!%3D%201%22%5D%3B%0D%0A%22State%20ID%3A%208%0D%0AAssignment%3A%20%7B'x'%3A%202%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%209%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22y%20%3D%3D%2010%22%5D%3B%0D%0A%22State%20ID%3A%209%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%2010%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2010%2C%20'z'%3A%20100%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%5D%7D%22%20%5Blabel%3D%22z%20%3D%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%209%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%2011%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2010%2C%20'z'%3A%20200%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B200%5D%7D%22%20%5Blabel%3D%22z%20!%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%208%0D%0AAssignment%3A%20%7B'x'%3A%202%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%2012%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22y%20!%3D%2010%22%5D%3B%0D%0A%22State%20ID%3A%2012%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%2013%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2020%2C%20'z'%3A%20100%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%5D%7D%22%20%5Blabel%3D%22z%20%3D%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%2012%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%2014%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2020%2C%20'z'%3A%20200%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B200%5D%7D%22%20%5Blabel%3D%22z%20!%3D%20100%22%5D%3B%0D%0A%7D).
 
 
 ## Install from PyPI
 
 Explorateur can be installed from PyPI using `pip install explorateur`
 
 ## Install from Source
@@ -133,20 +149,14 @@
 To confirm that installation was successful, try importing Explorateur after `pip install explorateur`
 
 ```
 import explorateur
 print(explorateur.__version__)
 ```
 
-## Changelog
-
-| Date         | Notes           |
-|--------------|-----------------|
-| 15 May, 2024 | Initial release |
-
 ## Support
 
 Please submit bug reports and feature requests as [Issues](https://github.com/explorateur/issues).
 
 ## License
 
 Explorateur is licensed under the [Apache License 2.0](LICENSE.md).
```

### Comparing `explorateur-1.1.0/explorateur/explorateur.py` & `explorateur-1.2.0/explorateur/explorateur.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,49 @@
 import copy as cp
 import time
 from typing import Optional, List, Tuple
 
 from explorateur._version import __version__
-from explorateur.search.decision import Decision
 from explorateur.search.exploration_type import ExplorationType
 from explorateur.search.search_type import SearchType
 from explorateur.search.transition import Transition
 from explorateur.state.base_state import BaseState
 from explorateur.state.storage.base_storage import BaseStorage
 from explorateur.state.storage.factory import StorageFactory
 from explorateur.utils import check_true, All_Exploration_Types, All_Search_Types, Constants
 
 __version__ = __version__
 
 
 class Explorateur:
     """
-    Explorateur is a Python library to conduct State-Space-Search (SSS).
-    SSS is useful for solving problems that require searching over a collection of states.
-    Explorateur starts with a given initial state, and then, performs iterative search moves until
-    either a termination state is found, the search space is exhausted, or a stopping criteria,
-    such as the number of iterations, runtime limit, or maximum depth, has been reached.
-    Optionally, a goal state can be given as input to terminate the search when the goal state is found.
-
-    Explorateur performs generic state space search over problem-specific `BaseState` and `BaseMove` representations.
-    The behavior of the overall algorithm is controlled by the search strategy and the exploration strategy.
-    The search strategy can be `TreeSearch` over open states, or
-    `GraphSearch` over open states while storing the closed on to avoid visiting duplicate states.
-    The exploration strategy can be uninformed as in `BreadthFirst` and `DepthFirst`, or
-    informed as in `BestFirst` that assumes an objective function to evaluate the solution quality of a state.
+        Explorateur is a Python library to conduct State-Space-Search (SSS).
+        SSS is a powerful framework for solving problems that require search over a collection of states.
+
+        Explorateur performs generic state-space-search over problem-specific states and moves.
+        The user defines the `BaseState` and `BaseMove` and the library drives the search for solutions.
+
+        Given an initial user state, Explorateur performs iterative search moves until a stopping condition is reached:
+            - A termination state is found
+            - The search space is exhausted
+            - Reached max iterations, runtime limit, max depth
+            - Optionally, given a goal state, a goal state is encountered.
+
+        The behavior of the overall algorithm is controlled by the Search Strategy and the Exploration Strategy.
+
+        Search Strategy:
+            - TreeSearch over open states
+            - GraphSearch over open states while also storing the closed states to avoid visiting duplicates.
+
+        Exploration Strategy:
+            - BreadthFirst in uninformed fashion
+            - DepthFirst in uninformed fashion
+            - BestFirst in informed fashion assuming an objective function evaluates the solution quality of a state.
+
+        To use Explorateur, you need to define BaseState and BaseMove, as in the quick start template.
     """
 
     def __init__(self, is_verbose=False):
         """ Initialize an Explorateur object. """
 
         # Validate arguments
         Explorateur._validate_args(is_verbose)
@@ -44,16 +54,16 @@
         self._log("[Explorateur v." + str(__version__) + "]")
 
         # Solution state
         self.solution_state: Optional[BaseState] = None
         self.solution_path: Optional[List[BaseState]] = None
 
         # State collections open and closed (for graph search only)
-        self._open_decisions: BaseStorage = None
-        self._closed_decisions: Optional[BaseStorage] = None
+        self._open: BaseStorage = None
+        self.closed: Optional[BaseStorage] = None
 
         # Statistics
         self._start_time: float = 0
         self.total_time: float = 0
         self.num_decisions: int = 0
         self.num_failed_decisions: int = 0
 
@@ -71,15 +81,15 @@
                max_moves: int = 10000,
                max_runtime: int = None,
                dot_filename: str = None) -> bool:
         """
         This function performs search from the initial_state until:
             - a solution found, or
             - goal_state reached if given, or
-            - termination criteria, in terms of number of seconds or iterations, is reached.
+            - stopping criteria, in terms of number of seconds, iterations, or depth, is reached.
 
         Arguments:
             - initial_state (BaseState): The initial state where the search will begin.
             - goal_state Optional(BaseState): Optional argument used for graph search to reach termination state.
                                               Default, None.
             - exploration_type Optional(ExplorationType): The exploration method.
                                                           Default, ExplorationType.DepthFirst().
@@ -95,183 +105,181 @@
             - max_runtime Optional(int): Optional argument for the number of seconds the search should go on for.
                                          Default, None (no limit).
             - dot_file_path (str): Optional argument to write a graph dot representation of search iterations.
                                    It uses logging CRITICAL level to log the dot output
                                    Default, None (no dot file saved).
                                    Example dot graph visualizer: https://dreampuf.github.io/GraphvizOnline/
         Returns:
-            - If no solution found or the search hits one of the stopping criteria,
-            returns None.
-            - if a solution is found and is_solution_path is set to False,
-            returns the solution state.
-            - If a solution is found, and is_solution_path is set to True,
-            returns a list of solution states, denoting the path from solution state back to the initial_state.
+            - If no solution found or the search hits one of the stopping criteria, returns False.
+            - if a solution is found and is_solution_path is set to False, returns the solution state.
+            - If a solution is found, and is_solution_path is set to True, returns a list of solution states,
+                denoting the path from solution state back to the initial_state.
         """
 
         # Check arguments
         self._log_start(">>> START SEARCH", max_depth, max_moves, max_runtime)
         Explorateur._validate_search_args(initial_state, goal_state,
                                           exploration_type, search_type, is_solution_path,
                                           max_depth, max_moves, max_runtime, dot_filename)
-        
+
         # Reset rng, solution_states, collections, dot graph, start time, stats
         self._reset_search(dot_filename)
 
         # Create storage for open states, and optionally, for closed states in graph search to avoid duplicate visits
-        self._open_decisions = StorageFactory.create(exploration_type)
-        self._closed_decisions = StorageFactory.create(search_type)
+        self._open = StorageFactory.create(exploration_type)
+        self.closed = StorageFactory.create(search_type)
 
         # Root node root from the given initial state
         root = cp.deepcopy(initial_state)
-        root._id = self.num_decisions
+        root.id = self.num_decisions
 
         # Check termination, else expand current state with possible moves
         # as open decisions for execution within depth
         is_terminate, is_solution = self._is_terminate_or_expand(root, goal_state, exploration_type, max_depth)
         if is_solution:
             if is_solution_path:
                 self.solution_path = self._get_solution_path()
             return True
         if is_terminate:
             return False
 
         # START SEARCH
-        while not self._open_decisions.is_empty():
+        while not self._open.is_empty():
             self.num_decisions += 1
             self._log("\nDecision " + str(self.num_decisions))
-            self._log("Open decisions: " + str(self._open_decisions.size()))
+            self._log("Open decisions: " + str(self._open.size()))
 
-            # Pop the current decision from open decisions for execution
-            current_decision = self._open_decisions.remove()
-            self._log("Current decision: " + str(current_decision))
+            # Pop the copied successor state from open for execution
+            successor = self._open.remove()
+            current = successor._transition.previous_state
+            move = successor._transition.move
+            self._log("Current decision: " + str(current))
 
             # Transition of the current state (there is no transition for initial moves)
-            transition = current_decision.state._transition
-            next_depth = transition.depth + 1 if transition else 1
-            self._log("Current transition: " + str(transition))
-
-            # Mark the decision as visited, if graph search
-            if self._closed_decisions:
-                self._log("Mark current decision as visited in closed decisions: " + str(self._closed_decisions.size()))
-                self._closed_decisions.insert(current_decision)
+            self._log("Current transition: " + str(current._transition))
 
             # Execute the move on a copy state
-            successor_state = cp.deepcopy(current_decision.state)
-            if successor_state.execute(current_decision.move):
+            if successor.execute(move):
                 self._log("Move is successful.")
 
-                # Set next depth and attach next transition to successor so that we can trace solution path
-                next_transition = Transition(previous_state=current_decision.state,
-                                             move=current_decision.move, depth=next_depth)
-                successor_state._transition = next_transition
-                successor_state._id = self.num_decisions - self.num_failed_decisions
-                self._log("Create next transition: " + str(next_transition) +
-                          " from ID: " + str(current_decision.state._id) + " to ID: " + str(successor_state._id))
-
-                # Create dot node transition
-                self._log_dot(current_decision, successor_state, color="")
-
-                # Check termination, else expand successor state with possible moves
-                # as open decisions for execution within depth
-                is_terminate, is_solution = self._is_terminate_or_expand(successor_state, goal_state, exploration_type, max_depth)
-                if is_solution:
-                    if is_solution_path:
-                        self.solution_path = self._get_solution_path()
-                    return True
-                if is_terminate:
-                    return False
+                successor.id = self.num_decisions - self.num_failed_decisions
+                self._log("Create next transition: " + str(successor._transition) +
+                          " from ID: " + str(current.id) + " to ID: " + str(successor.id))
+
+                # Mark the decision as visited, if graph search
+                if self.closed:
+                    self._log("Mark current decision as visited in closed decisions: " + str(self.closed.size()))
+                    self.closed.insert(current)
+
+                # Skip already visited successor, if graph search
+                if self.closed and self.closed.contains(successor):
+                    self._log("Skip adding decision. It is already visited. " + str(successor))
+                    self.num_decisions -= 1
+                else:
+                    # Create dot node transition
+                    self._log_dot(current, move, successor, color="")
+
+                    # Check termination, else expand successor state with possible moves for execution within depth
+                    is_terminate, is_solution = self._is_terminate_or_expand(successor, goal_state, exploration_type, max_depth)
+                    if is_solution:
+                        if is_solution_path:
+                            self.solution_path = self._get_solution_path()
+                        return True
+                    if is_terminate:
+                        return False
             else:
+                # Skip failed move and infeasible successor, reset failed transition
+                successor._transition = None
                 self.num_failed_decisions += 1
-                # Skip failed move and infeasible successor
                 self._log("Skip infeasible successor. Num fails: " + str(self.num_failed_decisions))
 
                 # Create dot node transition to a failed node
-                self._log_dot(current_decision, None, color=Constants.FAIL_NODE_COLOR)
+                self._log_dot(current, move, None, color=Constants.FAIL_NODE_COLOR)
 
             # Check stopping conditions before next iteration. If hits a limit, color last successor state
-            if self._is_search_limit(successor_state, self._start_time, self.num_decisions, max_runtime, max_moves):
+            if self._is_search_limit(successor, self._start_time, self.num_decisions, max_runtime, max_moves):
                 return False
 
         # No more open decisions left or limit reach and search finished, save the dot and return False
         self.total_time = time.perf_counter() - self._start_time
         self._log_finish("<<< FINISH SEARCH - FAILURE - No solution! ")
         self._log_dot_file()
         return False
 
-    def _is_search_limit(self, state, start, num_moves, max_runtime, max_moves):
-        # Check max_runtime
-        stop_cause = None
-        current_time = time.perf_counter()
-        if max_runtime is not None and current_time - start > max_runtime:
-            stop_cause = "Max runtime reached " + str(max_runtime)
-
-        # Check max_moves
-        if num_moves >= max_moves:
-            stop_cause = "Max number of moves reached " + str(max_moves)
-
-        # If stopped, log, save dot, and return None solution
-        if stop_cause:
-            self.total_time = current_time - start
-            self._log_finish("<<< FINISH SEARCH - STOP - No solution! " + stop_cause)
-            self._log_dot(None, state, color=Constants.LIMIT_NODE_COLOR)  # mark it green
-            self._log_dot_file()
-            return True
-        return False
-
     def _is_terminate_or_expand(self, state, goal_state, exploration_type, max_depth) -> Tuple[bool, bool]:
 
         is_terminate, is_solution = False, False
 
         # Check termination condition -- decided by the user state!
         if state.is_terminate(goal_state):
             is_terminate, is_solution = True, True
             self.solution_state = state
             self.total_time = time.perf_counter() - self._start_time
             self._log("Successful termination for state: " + str(state))
             self._log_finish("<<< FINISH SEARCH - SUCCESS - Solution Found!")
-            self._log_dot(None, state, color=Constants.SUCCESS_NODE_COLOR)  # mark it green
+            move = state._transition.move if state._transition else None
+            self._log_dot(None, move, state, color=Constants.SUCCESS_NODE_COLOR)  # mark it green
             self._log_dot_file()
             return is_terminate, is_solution
         else:
             self._log("Successor is not termination, add alternative moves")
 
         # If still within max depth bound, insert the successor into open states for exploration
         # Initial state does not have transition, so skip max depth for initial state
         if state._transition:
             if state._transition.depth >= max_depth:
                 # Don't terminate the whole search, but don't generate new open nodes
                 self._log("Max depth reached, not inserting new open node.")
-                self._log_dot(None, state, color=Constants.LIMIT_NODE_COLOR)
+                self._log_dot(None, state._transition.move, state, color=Constants.LIMIT_NODE_COLOR)
                 return is_terminate, is_solution
 
         # If no termination, add alternative moves to search -- decided by the user state!
         moves = state.get_moves()
 
         # Reverse moves for depth first search, so the exploration follows user move order
         if isinstance(exploration_type, ExplorationType.DepthFirst):
             moves.reverse()
 
         # Search for alternatives
         for move in moves:
             self._log("Decision for move: " + str(move))
 
-            # Create new decision
-            decision = Decision(state, move)
-
-            # Skip already visited successor, if graph search
-            if self._closed_decisions and self._closed_decisions.contains(decision):
-                self._log("Skip adding decision. It is already visited.")
-                continue
+            # Create a copy successor with next transition
+            successor_state = cp.deepcopy(state)
+            transition = state._transition
+            next_depth = transition.depth + 1 if transition else 1
+            next_transition = Transition(previous_state=state, move=move, depth=next_depth)
+            successor_state._transition = next_transition
 
             # Push successor to open storage for execution
-            self._log("Add open decision for executing " + str(decision.move) + " on state\n" + str(decision.state))
-            self._open_decisions.insert(decision)
+            self._log("Add open decision for executing " + str(successor_state._transition.move) + " on state\n" + str(state))
+            self._open.insert(successor_state)
 
         return is_terminate, is_solution
 
+    def _is_search_limit(self, state, start, num_moves, max_runtime, max_moves):
+        # Check max_runtime
+        stop_cause = None
+        current_time = time.perf_counter()
+        if max_runtime is not None and current_time - start > max_runtime:
+            stop_cause = "Max runtime reached " + str(max_runtime)
+
+        # Check max_moves
+        if num_moves >= max_moves:
+            stop_cause = "Max number of moves reached " + str(max_moves)
+
+        # If stopped, log, save dot, and return None solution
+        if stop_cause:
+            self.total_time = current_time - start
+            self._log_finish("<<< FINISH SEARCH - STOP - No solution! " + stop_cause)
+            self._log_dot(None, state._transition.move, state, color=Constants.LIMIT_NODE_COLOR)  # mark it green
+            self._log_dot_file()
+            return True
+        return False
+
     def _get_solution_path(self, is_initial_first=False) -> List[BaseState]:
         """
         Returns a list of states representing the order in which the search was performed.
 
         Args:
             - is_initial_first (bool): Indicates whether to reverse the path (list of states)
             so that the initial state is the first of the list.
@@ -316,32 +324,32 @@
         # Continue recursion from the previous internal state
         self._get_path_helper(transition.previous_state, state_list)
 
     def _log(self, text):
         if self.is_verbose:
             print(text)
 
-    def _log_dot(self, current_decision, successor_state, color):
+    def _log_dot(self, current, move, successor, color):
         if not self._dot_filename:
             return
 
-        if current_decision:
+        if current:
             # If there is no successor, first add a fail node with color so that we can add an edge to it
-            if not successor_state:
+            if not successor:
                 self._dot_text += (str(self.num_decisions) +
                                    " [label=\"Fail: " + str(self.num_failed_decisions) + "\"" +
                                    " shape=triangle style=filled fillcolor="+ str(color) + "];\n")
 
             # generic nodes with no color
-            self._dot_text += "\"" + current_decision.state.get_dot_label() + "\" -> "
-            self._dot_text += "\"" + successor_state.get_dot_label() + "\"" if successor_state else str(self.num_decisions)
-            self._dot_text += " [label=\"" + current_decision.move.get_dot_label() + "\"];\n"
+            self._dot_text += "\"" + current.get_dot_label() + "\" -> "
+            self._dot_text += "\"" + successor.get_dot_label() + "\"" if successor else str(self.num_decisions)
+            self._dot_text += " [label=\"" + move.get_dot_label() + "\"];\n"
         else:
             # decision is taken care of, mark successor with the color
-            self._dot_text += "\"" + successor_state.get_dot_label() + "\" [style=filled fillcolor=" + str(color) + "];\n"
+            self._dot_text += "\"" + successor.get_dot_label() + "\" [style=filled fillcolor=" + str(color) + "];\n"
 
     def _log_dot_file(self):
         if self._dot_filename:
             self._dot_text += "}"
             with open(self._dot_filename, 'w') as dot_file:
                 dot_file.write(self._dot_text)
 
@@ -360,16 +368,16 @@
     def _reset_search(self, dot_filename):
 
         # Clean solution states
         self.solution_state = None
         self.solution_path = None
 
         # Clean state collections
-        self._open_decisions = None
-        self._closed_decisions = None
+        self._open = None
+        self.closed = None
 
         # Initialize counters
         self._start_time = time.perf_counter()
         self.total_time = 0
         self.num_decisions = 0
         self.num_failed_decisions = 0
```

### Comparing `explorateur-1.1.0/explorateur/state/base_move.py` & `explorateur-1.2.0/explorateur/state/base_move.py`

 * *Files identical despite different names*

### Comparing `explorateur-1.1.0/explorateur/state/base_state.py` & `explorateur-1.2.0/explorateur/state/base_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,19 @@
     """
     Abstract class for the states.
     Model your problem as a state and transition between states via moves until termination.
     """
 
     @abc.abstractmethod
     def __init__(self):
-        """ 
+        """
         Initializer for state.
             For example, this can store variable and value assignments in the current state.
         """
-        self._id: int = -1
+        self.id: int = -1
         self._transition: Optional[Transition] = None
 
     @abc.abstractmethod
     def execute(self, move: BaseMove) -> bool:
         """
         Execute the given move on the state and return a boolean to denote successful (valid) execution.
 
@@ -80,8 +80,8 @@
         Best-First Search requires an evaluation of states for ranking.
 
         Note, if this function returns the same value for two states
         there will be an error because there is no comparator between abstract Base States.
 
         Returns:
             float: The objective function value for the state.
-        """
+        """
```

### Comparing `explorateur-1.1.0/explorateur/state/storage/factory.py` & `explorateur-1.2.0/explorateur/state/storage/factory.py`

 * *Files identical despite different names*

### Comparing `explorateur-1.1.0/explorateur/state/storage/priority_queue.py` & `explorateur-1.2.0/explorateur/state/storage/priority_queue.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import heapq
 from typing import List, Optional
 
-from explorateur.search.decision import Decision
 from explorateur.state.storage.base_storage import BaseStorage
+from explorateur.state.base_state import BaseState
 
 
 class PriorityQueue(BaseStorage):
     """  Class representing a priority queue. Root is the smallest element. """
 
     def __init__(self):
         super().__init__()
-        self.storage: List[Decision] = list()
+        self.storage: List[BaseState] = list()
 
-    def insert(self, decision: Decision):
-        heapq.heappush(self.storage, (decision.state.get_objective(), decision))
+    def insert(self, state: BaseState):
+        heapq.heappush(self.storage, (state.get_objective(), state))
 
-    def remove(self) -> Decision:
+    def remove(self) -> BaseState:
         """ Removes a state from the priority queue."""
         return heapq.heappop(self.storage)[1]  # the first item is the key
 
     def is_empty(self) -> bool:
         return len(self.storage) == 0
 
     def size(self) -> int:
         return len(self.storage)
 
-    def contains(self, decision: Decision) -> Optional[Decision]:
+    def contains(self, state: BaseState) -> Optional[BaseState]:
         """ Returns the state if it is in the priority queue, None otherwise."""
         try:
-            return self.storage[self.storage.index(decision)]
+            return self.storage[self.storage.index(state)]
         except ValueError:
             return None
```

### Comparing `explorateur-1.1.0/explorateur/state/storage/queue.py` & `explorateur-1.2.0/explorateur/state/storage/stack.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 from collections import deque
 from typing import Deque, Optional
-
-from explorateur.search.decision import Decision
 from explorateur.state.storage.base_storage import BaseStorage
+from explorateur.state.base_state import BaseState
 
 
-class Queue(BaseStorage):
-    """ Class representing a queue. """
+class Stack(BaseStorage):
+    """ Class representing a stack."""
 
     def __init__(self):
         super().__init__()
-        self.storage: Deque[Decision] = deque()
+        self.storage: Deque[BaseState] = deque()
 
-    def insert(self, decision: Decision):
-        self.storage.append(decision)
+    def insert(self, state: BaseState):
+        self.storage.append(state)
 
-    def remove(self) -> Decision:
-        return self.storage.popleft()
+    def remove(self) -> BaseState:
+        return self.storage.pop()
 
     def is_empty(self) -> bool:
-        return self.size() == 0
+        return len(self.storage) == 0
 
     def size(self) -> int:
         return len(self.storage)
 
-    def contains(self, decision: Decision) -> Optional[Decision]:
+    def contains(self, state: BaseState) -> Optional[BaseState]:
         """ Returns the state if it is in the stack, None otherwise."""
         try:
-            return self.storage[self.storage.index(decision)]
+            return self.storage[self.storage.index(state)]
         except ValueError:
             return None
```

### Comparing `explorateur-1.1.0/explorateur.egg-info/PKG-INFO` & `explorateur-1.2.0/explorateur.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: explorateur
-Version: 1.1.0
+Version: 1.2.0
 Summary: State space search
 Home-page: https://github.com/skadio/explorateur
 Author: xxx
 Project-URL: Documentation, https://xxx
 Project-URL: Source, https://xxx
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
+[![PyPI version fury.io](https://badge.fury.io/py/explorateur.svg)](https://pypi.python.org/pypi/explorateur/) [![PyPI license](https://img.shields.io/pypi/l/explorateur.svg)](https://pypi.python.org/pypi/explorateur/) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com) [![Downloads](https://static.pepy.tech/personalized-badge/explorateur?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/explorateur)
+
 # Explorateur
 
 Explorateur is a Python library to conduct [State-Space-Search (SSS)](https://en.wikipedia.org/wiki/State_space_search), a powerful framework for solving problems that require search over a collection of states. 
 
 Explorateur performs **generic state-space-search** over **problem-specific states and moves**. The user defines the `BaseState` and `BaseMove` and the library drives the search for solutions.
 
 Given an initial user state, Explorateur performs iterative search moves until a stopping condition is reached: 
@@ -33,29 +35,29 @@
 ### Exploration Strategy 
 - `BreadthFirst` in uninformed fashion 
 - `DepthFirst` in uninformed fashion
 - `BestFirst` in informed fashion assuming an objective function evaluates the solution quality of a state.
 
 ## Quick Start
 
-To use Explorateur, you need to define `BaseState` and `BaseMove`, with the quick start template below.  
+To use Explorateur, you need to define `BaseState` and `BaseMove` as in the template below.  
 
 ```python
 from explorateur import Explorateur, BaseMove, BaseState, ExplorationType, SearchType
 
 
 # TODO Implement your own Search Moves
 class MyMove(BaseMove):
 
     def __init__(self):
         # TODO Your move object
         pass
 
     def __str__(self) -> str:
-        # TODO Your mvoe string, also used for node labels in DOT graph
+        # TODO Your move string, also used for node labels in DOT graph
         pass
 
 
 # TODO Implement your own Search State 
 class MyState(BaseState):
 
     def __init__(self):
@@ -74,15 +76,15 @@
         # TODO Execute the move on the state and return success flag
         pass
 
     def __str__(self) -> str:
         # TODO Your state string, also used for node labels in DOT graph
         pass
 
-# Explorateur
+# Explarateur
 explorer = Explorateur()
 
 # Initial state
 initial_state = MyState()
 
 # Search for solutions
 if explorer.search(initial_state,
@@ -103,15 +105,15 @@
 print("Total Decisions:", explorer.num_decisions)
 print("Total Failures:", explorer.num_failed_decisions)
 print("Total Time:", explorer.total_time)
 ```
 
 ## Concrete Example
 
-Here is a concrete implementation to solve a toy [Constraint Satisfaction Problem](examples/usage_example.py) with the corresponding [search dot graph](examples/usage_example.dot)  and [search visualization](https://dreampuf.github.io/GraphvizOnline/#digraph%20G%20%7B%0D%0Aspline%3Dline%3B%0D%0A%22State%20ID%3A%200%0D%0AAssignment%3A%20%7B%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%2C%202%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%201%0D%0AAssignment%3A%20%7B'x'%3A%201%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22x%20%3D%3D%201%22%5D%3B%0D%0A%22State%20ID%3A%201%0D%0AAssignment%3A%20%7B'x'%3A%201%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%202%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22y%20%3D%3D%2010%22%5D%3B%0D%0A%22State%20ID%3A%202%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%203%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2010%2C%20'z'%3A%20100%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%5D%7D%22%20%5Blabel%3D%22z%20%3D%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%202%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%204%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2010%2C%20'z'%3A%20200%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B200%5D%7D%22%20%5Blabel%3D%22z%20!%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%201%0D%0AAssignment%3A%20%7B'x'%3A%201%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%205%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22y%20!%3D%2010%22%5D%3B%0D%0A%22State%20ID%3A%205%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%206%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2020%2C%20'z'%3A%20100%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%5D%7D%22%20%5Blabel%3D%22z%20%3D%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%205%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%207%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2020%2C%20'z'%3A%20200%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B200%5D%7D%22%20%5Blabel%3D%22z%20!%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%200%0D%0AAssignment%3A%20%7B%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%2C%202%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%208%0D%0AAssignment%3A%20%7B'x'%3A%202%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22x%20!%3D%201%22%5D%3B%0D%0A%22State%20ID%3A%208%0D%0AAssignment%3A%20%7B'x'%3A%202%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%209%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22y%20%3D%3D%2010%22%5D%3B%0D%0A%22State%20ID%3A%209%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%2010%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2010%2C%20'z'%3A%20100%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%5D%7D%22%20%5Blabel%3D%22z%20%3D%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%209%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%2011%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2010%2C%20'z'%3A%20200%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B200%5D%7D%22%20%5Blabel%3D%22z%20!%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%208%0D%0AAssignment%3A%20%7B'x'%3A%202%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%2012%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22y%20!%3D%2010%22%5D%3B%0D%0A%22State%20ID%3A%2012%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%2013%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2020%2C%20'z'%3A%20100%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%5D%7D%22%20%5Blabel%3D%22z%20%3D%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%2012%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%2014%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2020%2C%20'z'%3A%20200%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B200%5D%7D%22%20%5Blabel%3D%22z%20!%3D%20100%22%5D%3B%0D%0A%7D).
+Here is a concrete implementation to solve a toy [Constraint Satisfaction Problem](examples/backtrack_tree_search/main.py) using backtracking tree search, with the corresponding [search dot graph](examples/backtrack_tree_search/output.dot)  and [search visualization](https://dreampuf.github.io/GraphvizOnline/#digraph%20G%20%7B%0D%0Aspline%3Dline%3B%0D%0A%22State%20ID%3A%200%0D%0AAssignment%3A%20%7B%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%2C%202%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%201%0D%0AAssignment%3A%20%7B'x'%3A%201%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22x%20%3D%3D%201%22%5D%3B%0D%0A%22State%20ID%3A%201%0D%0AAssignment%3A%20%7B'x'%3A%201%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%202%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22y%20%3D%3D%2010%22%5D%3B%0D%0A%22State%20ID%3A%202%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%203%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2010%2C%20'z'%3A%20100%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%5D%7D%22%20%5Blabel%3D%22z%20%3D%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%202%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%204%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2010%2C%20'z'%3A%20200%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B200%5D%7D%22%20%5Blabel%3D%22z%20!%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%201%0D%0AAssignment%3A%20%7B'x'%3A%201%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%205%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22y%20!%3D%2010%22%5D%3B%0D%0A%22State%20ID%3A%205%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%206%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2020%2C%20'z'%3A%20100%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%5D%7D%22%20%5Blabel%3D%22z%20%3D%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%205%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%207%0D%0AAssignment%3A%20%7B'x'%3A%201%2C%20'y'%3A%2020%2C%20'z'%3A%20200%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B200%5D%7D%22%20%5Blabel%3D%22z%20!%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%200%0D%0AAssignment%3A%20%7B%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B1%2C%202%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%208%0D%0AAssignment%3A%20%7B'x'%3A%202%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22x%20!%3D%201%22%5D%3B%0D%0A%22State%20ID%3A%208%0D%0AAssignment%3A%20%7B'x'%3A%202%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%209%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22y%20%3D%3D%2010%22%5D%3B%0D%0A%22State%20ID%3A%209%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%2010%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2010%2C%20'z'%3A%20100%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%5D%7D%22%20%5Blabel%3D%22z%20%3D%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%209%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2010%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%2011%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2010%2C%20'z'%3A%20200%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%5D%2C%20'z'%3A%20%5B200%5D%7D%22%20%5Blabel%3D%22z%20!%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%208%0D%0AAssignment%3A%20%7B'x'%3A%202%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B10%2C%2020%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%2012%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20%5Blabel%3D%22y%20!%3D%2010%22%5D%3B%0D%0A%22State%20ID%3A%2012%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%2013%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2020%2C%20'z'%3A%20100%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%5D%7D%22%20%5Blabel%3D%22z%20%3D%3D%20100%22%5D%3B%0D%0A%22State%20ID%3A%2012%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2020%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B100%2C%20200%5D%7D%22%20-%3E%20%22State%20ID%3A%2014%0D%0AAssignment%3A%20%7B'x'%3A%202%2C%20'y'%3A%2020%2C%20'z'%3A%20200%7D%0D%0ADomains%3A%20%7B'x'%3A%20%5B2%5D%2C%20'y'%3A%20%5B20%5D%2C%20'z'%3A%20%5B200%5D%7D%22%20%5Blabel%3D%22z%20!%3D%20100%22%5D%3B%0D%0A%7D).
 
 
 ## Install from PyPI
 
 Explorateur can be installed from PyPI using `pip install explorateur`
 
 ## Install from Source
@@ -147,20 +149,14 @@
 To confirm that installation was successful, try importing Explorateur after `pip install explorateur`
 
 ```
 import explorateur
 print(explorateur.__version__)
 ```
 
-## Changelog
-
-| Date         | Notes           |
-|--------------|-----------------|
-| 15 May, 2024 | Initial release |
-
 ## Support
 
 Please submit bug reports and feature requests as [Issues](https://github.com/explorateur/issues).
 
 ## License
 
 Explorateur is licensed under the [Apache License 2.0](LICENSE.md).
```

### Comparing `explorateur-1.1.0/explorateur.egg-info/SOURCES.txt` & `explorateur-1.2.0/explorateur.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 LICENSE.md
-MANIFEST.in
 README.md
 setup.py
 explorateur/__init__.py
 explorateur/_version.py
 explorateur/explorateur.py
 explorateur/utils.py
 explorateur.egg-info/PKG-INFO
 explorateur.egg-info/SOURCES.txt
 explorateur.egg-info/dependency_links.txt
 explorateur.egg-info/top_level.txt
 explorateur/search/__init__.py
-explorateur/search/decision.py
 explorateur/search/exploration_type.py
 explorateur/search/search_type.py
 explorateur/search/storage.py
 explorateur/search/transition.py
 explorateur/state/__init__.py
 explorateur/state/base_move.py
 explorateur/state/base_state.py
```

### Comparing `explorateur-1.1.0/setup.py` & `explorateur-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `explorateur-1.1.0/tests/test_base.py` & `explorateur-1.2.0/tests/test_base.py`

 * *Files 15% similar despite different names*

```diff
@@ -38,30 +38,36 @@
         self.constraint: str = constraint
         self.val: int = val
 
     # String representation, also used for edge labels in DOT graph
     def __str__(self) -> str:
         return str(self.var) + " " + self.constraint + " " + str(self.val)
 
+    # This is required for graph search to check contains on already visited decisions
     def __eq__(self, other):
-        """Overrides the default implementation"""
         if isinstance(other, MyMove):
             return self.var == other.var and \
                 self.constraint == other.constraint and \
                 self.val == other.val
         return False
 
+    # This is required for graph search when adding closed decision into hashset
+    def __hash__(self):
+        return hash((self.var, self.constraint, self.val))
+
 
 class MyState(BaseState):
 
     # Problem specific state representation
-    def __init__(self, var_to_domain, is_exhaustive_search=True, fake_fails=[]):
+    def __init__(self, var_to_domain, is_exhaustive_search=True, fake_fails=None):
         # IMPORTANT: Make sure to initialize the base state
         super().__init__()
 
+        if fake_fails is None:
+            fake_fails = []
         self.var_to_domain: Dict[str, List[int]] = var_to_domain
         self.var_to_val: Dict[str, int] = {}
         self.unassigned: List[str] = list(self.var_to_domain.keys())
         self.is_exhaustive_search = is_exhaustive_search
         self.fake_fails = fake_fails
 
     # Design branching decisions
@@ -112,36 +118,40 @@
 
         # Successful execution
         print("USER Execute: SUCCESS")
         return True
 
     # String representation, also used for node labels in DOT graph
     def __str__(self) -> str:
-        text = "State ID: " + str(self._id) + "\n"
+        text = "State ID: " + str(self.id) + "\n"
         text += "Assignment: " + str(self.var_to_val) + "\n"
         text += "Domains: " + str(self.var_to_domain)
         return text
 
+    # This is required for graph search to check contains on already visited decisions
     def __eq__(self, other):
-        """Overrides the default implementation"""
         if isinstance(other, MyState):
             return self.unassigned == other.unassigned and \
                 self.var_to_val == other.var_to_val and \
                 self.var_to_domain == other.var_to_domain
         return False
 
+    # This is required for graph search when adding closed decision into hashset
+    def __hash__(self):
+        return hash((tuple(self.unassigned), tuple(self.var_to_val), tuple(self.var_to_domain)))
+
 
 class BaseTest(unittest.TestCase):
 
     def search(self,
-            explorer,
-            initial_state, goal_state,
-            exploration_type, search_type,
-            is_solution_path,
-            max_depth, max_moves, max_runtime, dot_filename, is_verbose):
+               explorer,
+               initial_state, goal_state,
+               exploration_type, search_type,
+               is_solution_path,
+               max_depth, max_moves, max_runtime, dot_filename, is_verbose):
 
         # Search for solutions
         if explorer.search(initial_state,
                            goal_state=goal_state,  # Optional goal state
                            exploration_type=exploration_type,
                            search_type=search_type,
                            is_solution_path=is_solution_path,
```

### Comparing `explorateur-1.1.0/tests/test_graph_best_first.py` & `explorateur-1.2.0/tests/test_graph_best_first.py`

 * *Files identical despite different names*

### Comparing `explorateur-1.1.0/tests/test_graph_breadth_first.py` & `explorateur-1.2.0/tests/test_tree_best_first.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,41 @@
 import os
 from explorateur.utils import Constants
 
 from tests.test_base import BaseTest, MyState, MyMove
 from explorateur import Explorateur, ExplorationType, SearchType
 
 
-class GraphBreadthTest(BaseTest):
+class TreeBestTest(BaseTest):
 
-    def test_graph_breadth_feasible(self):
+    def test_tree_best_feasible(self):
         # Explorateur
         explorer = Explorateur(is_verbose=True)
 
         # Initial state
         # Don't search the whole tree, stop at first feasible
         # Fake a few failing decisions
         initial_state = MyState({"x": [1, 2], "y": [10, 20], "z": [100, 200]},
                                 is_exhaustive_search=False)
-        # Search
-        self.search(explorer,
-                    initial_state,
-                    goal_state=None,
-                    exploration_type=ExplorationType.BreadthFirst(),
-                    search_type=SearchType.TreeSearch(),
-                    is_solution_path=True,
-                    max_depth=100,
-                    max_moves=100,
-                    max_runtime=100,
-                    dot_filename=os.path.join(Constants.TEST_DATA_DIR, "tree_breadth_first.dot"),
-                    is_verbose=True)
-
-        # Solution label
-        ground_truth_solution = {"x": 1, "y": 10, "z": 100}
-
-        self.assertEqual(explorer.num_decisions, 7)
-        self.assertEqual(explorer.num_failed_decisions, 0)
-        self.assertEqual(len(explorer.solution_path), 4)
-        self.assertEqual(explorer.solution_path[-1], initial_state)
-        self.assertEqual(explorer.solution_state.var_to_val, ground_truth_solution)
-        self.assertEqual(explorer.solution_state.unassigned, [])
+        # # Search
+        # self.search(explorer,
+        #             initial_state,
+        #             goal_state=None,
+        #             exploration_type=ExplorationType.DepthFirst(),
+        #             search_type=SearchType.TreeSearch(),
+        #             is_solution_path=True,
+        #             max_depth=100,
+        #             max_moves=100,
+        #             max_runtime=100,
+        #             dot_filename=os.path.join(Constants.TEST_DATA_DIR, "tree_best_first.dot"),
+        #             is_verbose=True)
+        #
+        # # Solution label
+        # ground_truth_solution = {"x": 1, "y": 10, "z": 100}
+        #
+        # self.assertEqual(explorer.num_decisions, 3)
+        # self.assertEqual(explorer.num_failed_decisions, 0)
+        # self.assertEqual(len(explorer.solution_path), 4)
+        # self.assertEqual(explorer.solution_path[-1], initial_state)
+        # self.assertEqual(explorer.solution_state.var_to_val, ground_truth_solution)
+        # self.assertEqual(explorer.solution_state.unassigned, [])
 
-    def test_graph_breadth_feasible_with_fakefails(self):
-        # Explorateur
-        explorer = Explorateur(is_verbose=True)
-
-        # Initial state
-        # Don't search the whole tree, stop at first feasible
-        # Fake a few failing decisions
-        initial_state = MyState({"x":[1,2], "y":[10, 20], "z":[100, 200]},
-                                is_exhaustive_search=False,
-                                fake_fails=[MyMove("x", "==", 1)])
-
-        # Search
-        self.search(explorer,
-                    initial_state,
-                    goal_state=None,
-                    exploration_type=ExplorationType.BreadthFirst(),
-                    search_type=SearchType.GraphSearch(),
-                    is_solution_path=True,
-                    max_depth=100,
-                    max_moves=100,
-                    max_runtime=100,
-                    dot_filename=os.path.join(Constants.TEST_DATA_DIR, "graph_breadth_first.dot"),
-                    is_verbose=True)
-
-        # Solution label
-        ground_truth_solution = {"x": 2, "y": 10, "z": 100}
-
-        self.assertEqual(explorer.num_decisions, 5)
-        self.assertEqual(explorer.num_failed_decisions, 1)
-        self.assertEqual(len(explorer.solution_path), 4)
-        self.assertEqual(explorer.solution_path[-1], initial_state)
-        self.assertEqual(explorer.solution_state.var_to_val, ground_truth_solution)
-        self.assertEqual(explorer.solution_state.unassigned, [])
```

### Comparing `explorateur-1.1.0/tests/test_invalid.py` & `explorateur-1.2.0/tests/test_invalid.py`

 * *Files identical despite different names*

### Comparing `explorateur-1.1.0/tests/test_storage.py` & `explorateur-1.2.0/tests/test_storage.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from tests.test_base import BaseTest, EmptyState
 from explorateur.state.storage.queue import Queue
 from explorateur.state.storage.stack import Stack
+from explorateur.state.storage.hash import HashSet
 from explorateur.state.storage.priority_queue import PriorityQueue
+from tests.test_base import BaseTest, MyState, MyMove
 
 
 class StorageState(EmptyState):
 
     def __init__(self, val):
         super().__init__()
         self.val = val
@@ -13,15 +15,15 @@
     def get_objective(self):
         if self.val == 2:
             return 1
         else:
             return 10
 
 
-class StorageTests(BaseTest):
+class StorageTest(BaseTest):
 
     # can't test for contains() because it takes in a _BaseState
     def test_queue(self):
         q = Queue()
         b1 = StorageState(1)
         b2 = StorageState(2)
         q.insert(b1)
@@ -41,14 +43,42 @@
         self.assertTrue(s.contains(b1))
         s.insert(b2)
         res = s.remove()
         self.assertEqual(b2, res)
         self.assertEqual(s.size(), 1)
         self.assertFalse(s.is_empty())
 
+    def test_hash(self):
+        state = MyState({"x": [1, 2], "y": [10, 20], "z": [100, 200]})
+        move = MyMove("x", "==", 1)
+
+        h = HashSet()
+        self.assertTrue(h.is_empty())
+
+        h.insert(state)
+        self.assertTrue(h.contains(state))
+        self.assertEqual(h.size(), 1)
+        self.assertFalse(h.is_empty())
+
+        d2 = MyState({"x": [1, 2], "y": [10, 20], "z": [100, 200]})
+        self.assertEqual(h.contains(d2), d2)
+
+        h.insert(d2)
+        self.assertEqual(h.size(), 1)
+
+        x = h.remove()
+        self.assertEqual(x, d2)
+        self.assertIsNone(h.contains(state))
+        self.assertTrue(h.is_empty())
+        self.assertEqual(h.size(), 0)
+
+        h.insert(state)
+        self.assertEqual(h.size(), 1)
+
+
     def test_priority_queue(self):
         # TODO
         pass
         # pq = PriorityQueue()
         # b1 = StorageState(1)
         # b2 = StorageState(2)
         # pq.insert(b1)
```

### Comparing `explorateur-1.1.0/tests/test_tree_best_first.py` & `explorateur-1.2.0/tests/test_graph_depth_first.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 import os
 from explorateur.utils import Constants
 
 from tests.test_base import BaseTest, MyState, MyMove
 from explorateur import Explorateur, ExplorationType, SearchType
+from explorateur.utils import run
 
 
-class TreeBestTest(BaseTest):
+class GraphDepthTest(BaseTest):
 
-    def test_tree_best_feasible(self):
+    def test_graph_depth_first(self):
         # Explorateur
         explorer = Explorateur(is_verbose=True)
 
         # Initial state
         # Don't search the whole tree, stop at first feasible
         # Fake a few failing decisions
         initial_state = MyState({"x": [1, 2], "y": [10, 20], "z": [100, 200]},
                                 is_exhaustive_search=False)
-        # # Search
-        # self.search(explorer,
-        #             initial_state,
-        #             goal_state=None,
-        #             exploration_type=ExplorationType.DepthFirst(),
-        #             search_type=SearchType.TreeSearch(),
-        #             is_solution_path=True,
-        #             max_depth=100,
-        #             max_moves=100,
-        #             max_runtime=100,
-        #             dot_filename=os.path.join(Constants.TEST_DATA_DIR, "tree_best_first.dot"),
-        #             is_verbose=True)
-        #
-        # # Solution label
-        # ground_truth_solution = {"x": 1, "y": 10, "z": 100}
-        #
-        # self.assertEqual(explorer.num_decisions, 3)
-        # self.assertEqual(explorer.num_failed_decisions, 0)
-        # self.assertEqual(len(explorer.solution_path), 4)
-        # self.assertEqual(explorer.solution_path[-1], initial_state)
-        # self.assertEqual(explorer.solution_state.var_to_val, ground_truth_solution)
-        # self.assertEqual(explorer.solution_state.unassigned, [])
 
+        # Arguments
+        args = {}
+        args["initial_state"] = initial_state
+        args["goal_state"] = None
+        args["exploration_type"] = ExplorationType.DepthFirst()
+        args["search_type"] = SearchType.GraphSearch()
+        args["is_solution_path"] = True
+        args["max_depth"] = 100
+        args["max_moves"] = 100
+        args["max_runtime"] = 100
+        args["dot_filename"] = os.path.join(Constants.TEST_DATA_DIR, "graph_depth_first.dot")
+        args["is_verbose"] = True
+
+        # Run
+        run(explorer, args)
+
+        # Solution label
+        ground_truth_solution = {"x": 1, "y": 10, "z": 100}
+        self.assertEqual(explorer.num_decisions, 3)
+        self.assertEqual(explorer.num_failed_decisions, 0)
+        self.assertEqual(len(explorer.solution_path), 4)
+        self.assertEqual(explorer.solution_path[-1], initial_state)
+        self.assertEqual(explorer.solution_state.var_to_val, ground_truth_solution)
+        self.assertEqual(explorer.solution_state.unassigned, [])
```

### Comparing `explorateur-1.1.0/tests/test_tree_breadth_first.py` & `explorateur-1.2.0/tests/test_tree_breadth_first.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 import os
 from explorateur.utils import Constants
 
 from tests.test_base import BaseTest, MyState, MyMove
 from explorateur import Explorateur, ExplorationType, SearchType
+from explorateur.utils import run
 
 
 class TreeBreadthTest(BaseTest):
 
     def test_tree_breadth_feasible(self):
         # Explorateur
         explorer = Explorateur(is_verbose=True)
 
         # Initial state
         # Don't search the whole tree, stop at first feasible
-        # Fake a few failing decisions
         initial_state = MyState({"x": [1, 2], "y": [10, 20], "z": [100, 200]},
                                 is_exhaustive_search=False)
-        # Search
-        self.search(explorer,
-                    initial_state,
-                    goal_state=None,
-                    exploration_type=ExplorationType.BreadthFirst(),
-                    search_type=SearchType.TreeSearch(),
-                    is_solution_path=True,
-                    max_depth=100,
-                    max_moves=100,
-                    max_runtime=100,
-                    dot_filename=os.path.join(Constants.TEST_DATA_DIR, "tree_breadth_first.dot"),
-                    is_verbose=True)
+
+        # Arguments
+        args = {}
+        args["initial_state"] = initial_state
+        args["goal_state"] = None
+        args["exploration_type"] = ExplorationType.BreadthFirst()
+        args["search_type"] = SearchType.TreeSearch()
+        args["is_solution_path"] = True
+        args["max_depth"] = 100
+        args["max_moves"] = 100
+        args["max_runtime"] = 100
+        args["dot_filename"] = os.path.join(Constants.TEST_DATA_DIR, "tree_breadth_first.dot")
+        args["is_verbose"] = True
+
+        # Run
+        run(explorer, args)
 
         # Solution label
         ground_truth_solution = {"x": 1, "y": 10, "z": 100}
-
         self.assertEqual(explorer.num_decisions, 7)
         self.assertEqual(explorer.num_failed_decisions, 0)
         self.assertEqual(len(explorer.solution_path), 4)
         self.assertEqual(explorer.solution_path[-1], initial_state)
         self.assertEqual(explorer.solution_state.var_to_val, ground_truth_solution)
         self.assertEqual(explorer.solution_state.unassigned, [])
 
@@ -46,29 +49,31 @@
         # Initial state
         # Don't search the whole tree, stop at first feasible
         # Fake a few failing decisions
         initial_state = MyState({"x":[1,2], "y":[10, 20], "z":[100, 200]},
                                 is_exhaustive_search=False,
                                 fake_fails=[MyMove("x", "==", 1)])
 
-        # Search
-        self.search(explorer,
-                    initial_state,
-                    goal_state=None,
-                    exploration_type=ExplorationType.BreadthFirst(),
-                    search_type=SearchType.TreeSearch(),
-                    is_solution_path=True,
-                    max_depth=100,
-                    max_moves=100,
-                    max_runtime=100,
-                    dot_filename=os.path.join(Constants.TEST_DATA_DIR, "tree_breadth_first.dot"),
-                    is_verbose=True)
+        # Arguments
+        args = {}
+        args["initial_state"] = initial_state
+        args["goal_state"] = None
+        args["exploration_type"] = ExplorationType.BreadthFirst()
+        args["search_type"] = SearchType.TreeSearch()
+        args["is_solution_path"] = True
+        args["max_depth"] = 100
+        args["max_moves"] = 100
+        args["max_runtime"] = 100
+        args["dot_filename"] = os.path.join(Constants.TEST_DATA_DIR, "tree_breadth_first.dot")
+        args["is_verbose"] = True
+
+        # Run
+        run(explorer, args)
 
         # Solution label
         ground_truth_solution = {"x": 2, "y": 10, "z": 100}
-
         self.assertEqual(explorer.num_decisions, 5)
         self.assertEqual(explorer.num_failed_decisions, 1)
         self.assertEqual(len(explorer.solution_path), 4)
         self.assertEqual(explorer.solution_path[-1], initial_state)
         self.assertEqual(explorer.solution_state.var_to_val, ground_truth_solution)
         self.assertEqual(explorer.solution_state.unassigned, [])
```

### Comparing `explorateur-1.1.0/tests/test_tree_depth_first.py` & `explorateur-1.2.0/tests/test_graph_breadth_first.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,75 +1,80 @@
 import os
 from explorateur.utils import Constants
 
 from tests.test_base import BaseTest, MyState, MyMove
 from explorateur import Explorateur, ExplorationType, SearchType
+from explorateur.utils import run
 
 
-class TreeDepthTest(BaseTest):
+class GraphBreadthTest(BaseTest):
 
-    def test_tree_depth_feasible(self):
+    def test_graph_breadth_feasible(self):
         # Explorateur
         explorer = Explorateur(is_verbose=True)
 
         # Initial state
         # Don't search the whole tree, stop at first feasible
         # Fake a few failing decisions
         initial_state = MyState({"x": [1, 2], "y": [10, 20], "z": [100, 200]},
                                 is_exhaustive_search=False)
-        # Search
-        self.search(explorer,
-                    initial_state,
-                    goal_state=None,
-                    exploration_type=ExplorationType.DepthFirst(),
-                    search_type=SearchType.TreeSearch(),
-                    is_solution_path=True,
-                    max_depth=100,
-                    max_moves=100,
-                    max_runtime=100,
-                    dot_filename=os.path.join(Constants.TEST_DATA_DIR, "tree_depth_first.dot"),
-                    is_verbose=True)
+        # Arguments
+        args = {}
+        args["initial_state"] = initial_state
+        args["goal_state"] = None
+        args["exploration_type"] = ExplorationType.BreadthFirst()
+        args["search_type"] = SearchType.GraphSearch()
+        args["is_solution_path"] = True
+        args["max_depth"] = 100
+        args["max_moves"] = 100
+        args["max_runtime"] = 100
+        args["dot_filename"] = os.path.join(Constants.TEST_DATA_DIR, "tree_breadth_first.dot")
+        args["is_verbose"] = True
+
+        # Run
+        run(explorer, args)
 
         # Solution label
         ground_truth_solution = {"x": 1, "y": 10, "z": 100}
 
-        self.assertEqual(explorer.num_decisions, 3)
+        self.assertEqual(explorer.num_decisions, 7)
         self.assertEqual(explorer.num_failed_decisions, 0)
         self.assertEqual(len(explorer.solution_path), 4)
         self.assertEqual(explorer.solution_path[-1], initial_state)
         self.assertEqual(explorer.solution_state.var_to_val, ground_truth_solution)
         self.assertEqual(explorer.solution_state.unassigned, [])
 
-    def test_tree_depth_feasible_with_fakefails(self):
-
+    def test_graph_breadth_feasible_with_fakefails(self):
         # Explorateur
         explorer = Explorateur(is_verbose=True)
 
         # Initial state
         # Don't search the whole tree, stop at first feasible
         # Fake a few failing decisions
         initial_state = MyState({"x":[1,2], "y":[10, 20], "z":[100, 200]},
                                 is_exhaustive_search=False,
-                                fake_fails=[MyMove("x", "==", 1), MyMove("z", "==", 100)])
+                                fake_fails=[MyMove("x", "==", 1)])
 
-        # Search
-        self.search(explorer,
-                    initial_state,
-                    goal_state=None,
-                    exploration_type=ExplorationType.DepthFirst(),
-                    search_type=SearchType.TreeSearch(),
-                    is_solution_path=True,
-                    max_depth=100,
-                    max_moves=100,
-                    max_runtime=100,
-                    dot_filename=os.path.join(Constants.TEST_DATA_DIR, "tree_depth_first.dot"),
-                    is_verbose=True)
+        # Arguments
+        args = {}
+        args["initial_state"] = initial_state
+        args["goal_state"] = None
+        args["exploration_type"] = ExplorationType.BreadthFirst()
+        args["search_type"] = SearchType.GraphSearch()
+        args["is_solution_path"] = True
+        args["max_depth"] = 100
+        args["max_moves"] = 100
+        args["max_runtime"] = 100
+        args["dot_filename"] = os.path.join(Constants.TEST_DATA_DIR, "graph_breadth_first.dot")
+        args["is_verbose"] = True
 
-        # Solution label
-        ground_truth_solution = {"x": 2, "y": 10, "z": 200}
+        # Run
+        run(explorer, args)
 
+        # Solution label
+        ground_truth_solution = {"x": 2, "y": 10, "z": 100}
         self.assertEqual(explorer.num_decisions, 5)
-        self.assertEqual(explorer.num_failed_decisions, 2)
+        self.assertEqual(explorer.num_failed_decisions, 1)
         self.assertEqual(len(explorer.solution_path), 4)
         self.assertEqual(explorer.solution_path[-1], initial_state)
         self.assertEqual(explorer.solution_state.var_to_val, ground_truth_solution)
-        self.assertEqual(explorer.solution_state.unassigned, [])
+        self.assertEqual(explorer.solution_state.unassigned, [])
```

