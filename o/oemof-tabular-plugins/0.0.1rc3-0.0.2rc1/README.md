# Comparing `tmp/oemof-tabular-plugins-0.0.1rc3.tar.gz` & `tmp/oemof_tabular_plugins-0.0.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oemof-tabular-plugins-0.0.1rc3.tar", last modified: Tue Apr  9 13:43:39 2024, max compression
+gzip compressed data, was "oemof_tabular_plugins-0.0.2rc1.tar", last modified: Tue May 21 14:01:01 2024, max compression
```

## Comparing `oemof-tabular-plugins-0.0.1rc3.tar` & `oemof_tabular_plugins-0.0.2rc1.tar`

### file list

```diff
@@ -1,40 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 13:43:39.710360 oemof-tabular-plugins-0.0.1rc3/
--rw-rw-rw-   0        0        0     1101 2024-02-12 12:09:55.000000 oemof-tabular-plugins-0.0.1rc3/LICENSE.txt
--rw-rw-rw-   0        0        0     4184 2024-04-09 13:43:39.706359 oemof-tabular-plugins-0.0.1rc3/PKG-INFO
--rw-rw-rw-   0        0        0     3478 2024-02-28 09:13:04.000000 oemof-tabular-plugins-0.0.1rc3/README.rst
--rw-rw-rw-   0        0        0     1028 2024-02-28 09:18:36.000000 oemof-tabular-plugins-0.0.1rc3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-09 13:43:39.586177 oemof-tabular-plugins-0.0.1rc3/requirements/
--rw-rw-rw-   0        0        0      135 2024-04-09 13:37:59.000000 oemof-tabular-plugins-0.0.1rc3/requirements/build_requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 13:43:39.710360 oemof-tabular-plugins-0.0.1rc3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-09 13:43:39.566499 oemof-tabular-plugins-0.0.1rc3/src/
-drwxrwxrwx   0        0        0        0 2024-04-09 13:43:39.593178 oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins/
--rw-rw-rw-   0        0        0      278 2024-02-28 09:13:04.000000 oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins/__init__.py
--rw-rw-rw-   0        0        0       49 2024-04-09 13:41:46.000000 oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins/_version.py
-drwxrwxrwx   0        0        0        0 2024-04-09 13:43:39.644929 oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins/general/
--rw-rw-rw-   0        0        0      145 2024-04-09 13:32:43.000000 oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins/general/__init__.py
--rw-rw-rw-   0        0        0     1027 2024-02-28 09:13:04.000000 oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins/general/constraint_facades.py
--rw-rw-rw-   0        0        0     1075 2024-02-28 09:13:04.000000 oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins/general/constraints.py
--rw-rw-rw-   0        0        0    25522 2024-03-21 14:12:59.000000 oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins/general/post_processing.py
--rw-rw-rw-   0        0        0     9114 2024-03-13 09:01:01.000000 oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins/general/pre_processing.py
-drwxrwxrwx   0        0        0        0 2024-04-09 13:43:39.662933 oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins/hydrogen/
--rw-rw-rw-   0        0        0       57 2024-02-28 09:13:04.000000 oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins/hydrogen/__init__.py
--rw-rw-rw-   0        0        0       24 2024-02-28 09:13:04.000000 oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins/hydrogen/constraint_facades.py
--rw-rw-rw-   0        0        0        0 2024-02-28 09:13:04.000000 oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins/hydrogen/constraints.py
--rw-rw-rw-   0        0        0       48 2024-02-28 09:13:04.000000 oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins/hydrogen/post_processing.py
-drwxrwxrwx   0        0        0        0 2024-04-09 13:43:39.677936 oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins/wefe/
--rw-rw-rw-   0        0        0       57 2024-02-28 09:13:04.000000 oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins/wefe/__init__.py
--rw-rw-rw-   0        0        0       24 2024-02-28 09:13:04.000000 oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins/wefe/constraint_facades.py
--rw-rw-rw-   0        0        0        0 2024-02-28 09:13:04.000000 oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins/wefe/constraints.py
-drwxrwxrwx   0        0        0        0 2024-04-09 13:43:39.690356 oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins/wefe/facades/
--rw-rw-rw-   0        0        0       35 2024-04-09 13:32:43.000000 oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins/wefe/facades/__init__.py
--rw-rw-rw-   0        0        0     4823 2024-03-13 09:01:01.000000 oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins/wefe/facades/pv_panel.py
--rw-rw-rw-   0        0        0       89 2024-02-28 09:13:04.000000 oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins/wefe/post_processing.py
-drwxrwxrwx   0        0        0        0 2024-04-09 13:43:39.702358 oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins.egg-info/
--rw-rw-rw-   0        0        0     4184 2024-04-09 13:43:39.000000 oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1232 2024-04-09 13:43:39.000000 oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 13:43:39.000000 oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-04-09 13:43:39.000000 oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-04-09 13:43:39.000000 oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-04-09 13:43:39.000000 oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-09 13:43:39.697357 oemof-tabular-plugins-0.0.1rc3/tests/
--rw-rw-rw-   0        0        0      625 2024-04-09 09:45:06.000000 oemof-tabular-plugins-0.0.1rc3/tests/test_pre_processing.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:01:01.569268 oemof_tabular_plugins-0.0.2rc1/
+-rw-rw-rw-   0        0        0     1101 2024-02-12 12:09:55.000000 oemof_tabular_plugins-0.0.2rc1/LICENSE.txt
+-rw-rw-rw-   0        0        0     4249 2024-05-21 14:01:01.565268 oemof_tabular_plugins-0.0.2rc1/PKG-INFO
+-rw-rw-rw-   0        0        0     3543 2024-05-21 13:58:23.000000 oemof_tabular_plugins-0.0.2rc1/README.rst
+-rw-rw-rw-   0        0        0     1030 2024-05-21 09:32:56.000000 oemof_tabular_plugins-0.0.2rc1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-21 14:01:01.435701 oemof_tabular_plugins-0.0.2rc1/requirements/
+-rw-rw-rw-   0        0        0      135 2024-04-09 14:16:30.000000 oemof_tabular_plugins-0.0.2rc1/requirements/build_requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 14:01:01.570268 oemof_tabular_plugins-0.0.2rc1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-21 14:01:01.415696 oemof_tabular_plugins-0.0.2rc1/src/
+drwxrwxrwx   0        0        0        0 2024-05-21 14:01:01.443358 oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins/
+-rw-rw-rw-   0        0        0      276 2024-05-21 13:54:43.000000 oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins/__init__.py
+-rw-rw-rw-   0        0        0       51 2024-05-21 13:56:48.000000 oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins/_version.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:01:01.474579 oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins/datapackage/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:32:57.000000 oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins/datapackage/__init__.py
+-rw-rw-rw-   0        0        0     1891 2024-05-21 09:32:57.000000 oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins/datapackage/building.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:01:01.507844 oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins/general/
+-rw-rw-rw-   0        0        0      190 2024-05-21 13:54:43.000000 oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins/general/__init__.py
+-rw-rw-rw-   0        0        0     1031 2024-05-21 13:54:43.000000 oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins/general/constraint_facades.py
+-rw-rw-rw-   0        0        0     1135 2024-05-21 13:54:43.000000 oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins/general/constraints.py
+-rw-rw-rw-   0        0        0    26545 2024-05-21 13:54:43.000000 oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins/general/post_processing.py
+-rw-rw-rw-   0        0        0      167 2024-05-21 13:54:43.000000 oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins/general/post_processing_moo.py
+-rw-rw-rw-   0        0        0    20212 2024-05-21 13:54:43.000000 oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins/general/pre_processing.py
+-rw-rw-rw-   0        0        0     1618 2024-05-21 13:54:43.000000 oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins/general/pre_processing_moo.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:01:01.522964 oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins/hydrogen/
+-rw-rw-rw-   0        0        0       53 2024-05-21 13:54:43.000000 oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins/hydrogen/__init__.py
+-rw-rw-rw-   0        0        0       26 2024-05-21 13:54:43.000000 oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins/hydrogen/constraint_facades.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 13:54:43.000000 oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins/hydrogen/constraints.py
+-rw-rw-rw-   0        0        0       50 2024-05-21 13:54:43.000000 oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins/hydrogen/post_processing.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:01:01.536260 oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins/wefe/
+-rw-rw-rw-   0        0        0       53 2024-05-21 13:54:43.000000 oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins/wefe/__init__.py
+-rw-rw-rw-   0        0        0       26 2024-05-21 13:54:43.000000 oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins/wefe/constraint_facades.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 13:54:43.000000 oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins/wefe/constraints.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:01:01.545263 oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins/wefe/facades/
+-rw-rw-rw-   0        0        0       31 2024-05-21 09:32:57.000000 oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins/wefe/facades/__init__.py
+-rw-rw-rw-   0        0        0     4859 2024-05-21 09:32:57.000000 oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins/wefe/facades/pv_panel.py
+-rw-rw-rw-   0        0        0       93 2024-05-21 13:54:43.000000 oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins/wefe/post_processing.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:01:01.559267 oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins.egg-info/
+-rw-rw-rw-   0        0        0     4249 2024-05-21 14:01:01.000000 oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1445 2024-05-21 14:01:01.000000 oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 14:01:01.000000 oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-21 14:01:01.000000 oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-05-21 14:01:01.000000 oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-05-21 14:01:01.000000 oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 14:01:01.553265 oemof_tabular_plugins-0.0.2rc1/tests/
+-rw-rw-rw-   0        0        0    28289 2024-05-21 09:32:57.000000 oemof_tabular_plugins-0.0.2rc1/tests/test_pre_processing.py
```

### Comparing `oemof-tabular-plugins-0.0.1rc3/LICENSE.txt` & `oemof_tabular_plugins-0.0.2rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oemof-tabular-plugins-0.0.1rc3/PKG-INFO` & `oemof_tabular_plugins-0.0.2rc1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: oemof-tabular-plugins
-Version: 0.0.1rc3
-Summary: A package that contains various constraint facades to be used with oemof-tabular
-Author-email: Ciara Dunks <ciara.dunks@rl-institut.de>, Pierre-François Duc <pierre-francois.duc@rl-institut.de>
-Project-URL: Homepage, https://github.com/rl-institut/oemof-tabular-plugins
-Project-URL: Issues, https://github.com/rl-institut/oemof-tabular-plugins/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
-License-File: LICENSE.txt
-Requires-Dist: oemof-tabular
-
 
 .. figure:: https://user-images.githubusercontent.com/14353512/185425447-85dbcde9-f3a2-4f06-a2db-0dee43af2f5f.png
     :align: left
     :target: https://github.com/rl-institut/super-repo/
     :alt: Repo logo
 
 =====================
@@ -29,19 +14,19 @@
    :widths: auto
 
    * - License
      - |badge_license|
    * - Documentation
      - |badge_documentation|
    * - Publication
-     - 
+     -
    * - Development
-     - |badge_issue_open| |badge_issue_closes| |badge_pr_open| |badge_pr_closes|
+     - |badge_issue_open| |badge_issue_closes| |badge_pr_open| |badge_pr_closes| |badge_black|
    * - Community
-     - |badge_contributing| |badge_contributors| |badge_repo_counts|
+     - |badge_contributing| |badge_contributors|
 
 .. contents::
     :depth: 2
     :local:
     :backlinks: top
 
 Introduction
@@ -83,24 +68,25 @@
 .. |badge_documentation| image:: https://img.shields.io/github/actions/workflow/status/rl-institut/super-repo/gh-pages.yml?branch=production
     :target: https://rl-institut.github.io/super-repo/
     :alt: Documentation
 
 .. |badge_contributing| image:: https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat
     :alt: contributions
 
-.. |badge_repo_counts| image:: http://hits.dwyl.com/rl-institut/super-repo.svg
-    :alt: counter
-
 .. |badge_contributors| image:: https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square
     :alt: contributors
 
 .. |badge_issue_open| image:: https://img.shields.io/github/issues-raw/rl-institut/super-repo
     :alt: open issues
 
 .. |badge_issue_closes| image:: https://img.shields.io/github/issues-closed-raw/rl-institut/super-repo
     :alt: closes issues
 
 .. |badge_pr_open| image:: https://img.shields.io/github/issues-pr-raw/rl-institut/super-repo
-    :alt: closes issues
+    :alt: open pull requests
 
 .. |badge_pr_closes| image:: https://img.shields.io/github/issues-pr-closed-raw/rl-institut/super-repo
-    :alt: closes issues
+    :alt: closes pull requests
+
+.. |badge_black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: black linting badge
```

### Comparing `oemof-tabular-plugins-0.0.1rc3/pyproject.toml` & `oemof_tabular_plugins-0.0.2rc1/pyproject.toml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 dependencies = {file = ["requirements/build_requirements.txt"]}
 
 [project.scripts]
 cli-name = "mypkg.mymodule:some_func"
 
 [project.urls]
 Homepage = "https://github.com/rl-institut/oemof-tabular-plugins"
-Issues = "https://github.com/rl-institut/oemof-tabular-plugins/issues"
+Issues = "https://github.com/rl-institut/oemof-tabular-plugins/issues"
```

### Comparing `oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins/general/constraint_facades.py` & `oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins/general/constraint_facades.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dataclasses import dataclass
 from oemof.tabular.constraint_facades import ConstraintFacade
 from .constraints import renewable_share_minimum
 
+
 @dataclass
 class MinimumRenewableShare(ConstraintFacade):
     name: str
     type: str
     limit: float
     keyword: str = "renewable_factor"
 
@@ -15,14 +16,15 @@
         flows = {}
         for i, o in model.flows:
             if hasattr(model.flows[i, o], self.keyword):
                 flows[(i, o)] = model.flows[i, o]
 
         if not flows:
             raise Warning(f"No flows with keyword {self.keyword}")
-        #else:
-            #print(f"These flows will contribute to the integral limit: {flows.keys()}")
+        # else:
+        # print(f"These flows will contribute to the integral limit: {flows.keys()}")
 
         # Add constraint to the model
         renewable_share_minimum(model, flows=flows, limit=self.limit)
 
-CONSTRAINT_TYPE_MAP = {"minimum_renewable_share": MinimumRenewableShare}
+
+CONSTRAINT_TYPE_MAP = {"minimum_renewable_share": MinimumRenewableShare}
```

### Comparing `oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins/general/constraints.py` & `oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins/general/constraints.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 from pyomo import environ as po
 
+
 def renewable_share_minimum(model, flows=None, limit=None):
     keyword = "renewable_factor"
 
     if flows is None:
         flows = {}
-        for (i, o) in model.flows:
+        for i, o in model.flows:
             if hasattr(model.flows[i, o], keyword):
                 flows[(i, o)] = model.flows[i, o]
     else:
-        for (i, o) in flows:
+        for i, o in flows:
             if not hasattr(flows[i, o], keyword):
                 raise AttributeError(
                     f"Flow with source: {i.label} and target: {o.label} has no attribute {keyword}."
                 )
     # this structure only works if you don't use multi-period
-    total_generation = sum(model.flow[i, o, 0, t] for (i, o) in flows for t in model.TIMESTEPS)
+    total_generation = sum(
+        model.flow[i, o, 0, t] for (i, o) in flows for t in model.TIMESTEPS
+    )
     renewable_generation = sum(
-        model.flow[i, o, 0, t] * getattr(flows[i, o], keyword) for (i, o) in flows for t in model.TIMESTEPS
+        model.flow[i, o, 0, t] * getattr(flows[i, o], keyword)
+        for (i, o) in flows
+        for t in model.TIMESTEPS
     )
     constraint_name = "renewable_share_minimum_constraint"
-    model.add_component(constraint_name, po.Constraint(expr=(renewable_generation >= float(limit) * total_generation)))
+    model.add_component(
+        constraint_name,
+        po.Constraint(expr=(renewable_generation >= float(limit) * total_generation)),
+    )
 
-    return model
+    return model
```

### Comparing `oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins/general/post_processing.py` & `oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins/general/post_processing.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,34 +5,36 @@
 import warnings
 from oemof.tabular.postprocessing.core import Calculator
 from oemof.tabular.postprocessing import calculations as clc, naming
 
 
 def excess_generation(all_scalars):
     # assuming your DataFrame has a MultiIndex with levels ("name", "var_name")
-    excess_rows = all_scalars[all_scalars.index.get_level_values("name").str.contains('excess')]
+    excess_rows = all_scalars[
+        all_scalars.index.get_level_values("name").str.contains("excess")
+    ]
     # convert the excess_rows DataFrame to a dictionary
-    excess_dict = excess_rows['var_value'].to_dict()
+    excess_dict = excess_rows["var_value"].to_dict()
     # extract only the first part of the MultiIndex ('name') and use it as the key
     excess_dict = {(key[0]): value for key, value in excess_dict.items()}
 
     return excess_dict
 
 
 def specific_system_costs(all_scalars, total_system_costs):
     """
     Calculates the specific system costs based on total system costs (this might change) and total demand in
     MWh (including demands from all sectors)
     :return:
     """
     # conditionally extract values based on the 'type' column
-    demand_values = all_scalars.loc[all_scalars['type'] == 'load', 'var_value'].tolist()
+    demand_values = all_scalars.loc[all_scalars["type"] == "load", "var_value"].tolist()
     demand_values_sum = sum(demand_values)
     # extract total_system_cost value from dataframe
-    total_system_cost = total_system_costs['var_value'].iloc[0]
+    total_system_cost = total_system_costs["var_value"].iloc[0]
     # calculate specific system costs (currency/kWh)
     specific_system_cost = total_system_cost / demand_values_sum / 1000
 
     return specific_system_cost
 
 
 def calculate_renewable_share(results):
@@ -45,21 +47,23 @@
     # initiate renewable_generation and nonrenewable_generation values
     renewable_generation = 0
     nonrenewable_generation = 0
 
     # loop through the results dict
     for entry_key, entry_value in results.items():
         # store the 'sequences' value for each oemof object tuple in results dict
-        sequences = entry_value.get('sequences', None)
+        sequences = entry_value.get("sequences", None)
         # check if the oemof object tuple has the 'output_parameters' attribute
-        if hasattr(entry_key[0], 'output_parameters'):
+        if hasattr(entry_key[0], "output_parameters"):
             # store the 'output_parameters' dict as output_param_dict
             output_param_dict = entry_key[0].output_parameters
             # retrieve the 'renewable_factor' value
-            renewable_factor = output_param_dict.get('custom_attributes', {}).get('renewable_factor')
+            renewable_factor = output_param_dict.get("custom_attributes", {}).get(
+                "renewable_factor"
+            )
             # if the renewable factor is 0, add the sum of flows to nonrenewable_generation
             if renewable_factor == 0:
                 nonrenewable_generation += sequences.sum().sum()
             # if the renewable factor is 1, add the sum of flows to renewable_generation
             elif renewable_factor == 1:
                 renewable_generation += sequences.sum().sum()
         else:
@@ -67,18 +71,20 @@
             nonrenewable_generation += 0
             renewable_generation += 0
 
     # calculate the total generation
     total_generation = renewable_generation + nonrenewable_generation
     # if total generation is 0, return 0 to avoid division by 0
     if total_generation == 0:
-        warning_message = "Total generation is 0. This may be because there is no generation or the" \
-                          " renewable factor is not defined in the output parameters of the inputs."
+        warning_message = (
+            "Total generation is 0. This may be because there is no generation or the"
+            " renewable factor is not defined in the output parameters of the inputs."
+        )
         warnings.warn(warning_message, UserWarning)
-    return 0
+        return 0
     # calculate the renewable share (rounded to 2dp)
     renewable_share = round(renewable_generation / total_generation, 2)
 
     return renewable_share
 
 
 def calculate_total_emissions(results):
@@ -89,283 +95,367 @@
     """
     # initiate total emissions value
     total_emissions = 0
 
     # loop through the results dict
     for entry_key, entry_value in results.items():
         # store the 'sequences' value for each oemof object tuple in results dict
-        sequences = entry_value.get('sequences', None)
+        sequences = entry_value.get("sequences", None)
         # check if the oemof object tuple has the 'output_parameters' attribute
-        if hasattr(entry_key[0], 'output_parameters'):
+        if hasattr(entry_key[0], "output_parameters"):
             # store the 'output_parameters' dict as output_param_dict
             output_param_dict = entry_key[0].output_parameters
             # retrieve the 'specific_emission' value if it exists
-            specific_emission = output_param_dict.get('custom_attributes', {}).get('specific_emission')
+            specific_emission = output_param_dict.get("custom_attributes", {}).get(
+                "specific_emission"
+            )
             if specific_emission is not None:
                 total_emissions += specific_emission * sequences.sum().sum()
                 logging.info(f"Specific emissions recorded for {entry_key}")
     # round the total emissions to 2dp
     total_emissions = round(total_emissions, 2)
 
     return total_emissions
 
 
 def create_capacities_table(all_scalars, results):
     # ToDo: maybe there is a way to make this function cleaner/shorter
     # set columns of the capacities dataframe
     capacities_df = pd.DataFrame(
-        columns=['Component', 'Type', 'Carrier', 'Existing Capacity', 'Capacity Potential', 'Optimizable',
-                 'Optimized Capacity'])
+        columns=[
+            "Component",
+            "Type",
+            "Carrier",
+            "Existing Capacity",
+            "Capacity Potential",
+            "Optimizable",
+            "Optimized Capacity",
+        ]
+    )
     # create an empty set for the component names
     component_names = set()
     # iterate over the index and row of the dataframe
     for idx, row in all_scalars.iterrows():
         # store variables to be included in the dataframe
         component_name = idx[0]
         component_variable = idx[1]
-        component_type = row['type']
-        component_carrier = row['carrier']
+        component_type = row["type"]
+        component_carrier = row["carrier"]
         # only include component names that haven't already been included to avoid repetition,
         # and don't include system in the dataframe because this refers to the system costs (nothing with capacities)
         # and don't include the storage components because these are stored in a different table
-        if component_name not in component_names and component_name != 'system' and 'storage' not in component_name:
+        if (
+            component_name not in component_names
+            and component_name != "system"
+            and "storage" not in component_name
+        ):
             component_names.add(component_name)
             # add component name and corresponding type and carrier to the dataframe
-            capacities_df = capacities_df._append({'Component': component_name,
-                                                   'Type': component_type,
-                                                   'Carrier': component_carrier}, ignore_index=True)
+            capacities_df = capacities_df._append(
+                {
+                    "Component": component_name,
+                    "Type": component_type,
+                    "Carrier": component_carrier,
+                },
+                ignore_index=True,
+            )
 
         # check if 'invest_out' is in the component_variable
-        if 'invest_out' in component_variable:
+        if "invest_out" in component_variable:
             # if it is, get the corresponding 'var_value' for the optimized capacity value
-            component_opt_capacity = row['var_value']
+            component_opt_capacity = row["var_value"]
             # if the value is -0.0, adapt this to 0.0
             if component_opt_capacity == -0.0:
                 component_opt_capacity = 0.0
             # add or update 'Optimized Capacity' for the component_name with the optimized capacity value
             capacities_df.loc[
-                capacities_df['Component'] == component_name, 'Optimized Capacity'] = component_opt_capacity
+                capacities_df["Component"] == component_name, "Optimized Capacity"
+            ] = component_opt_capacity
 
     # loop through the results dict
     for entry_key, entry_value in results.items():
         # check if the oemof object tuple has the 'capacity' attribute
-        if hasattr(entry_key[0], 'capacity'):
+        if hasattr(entry_key[0], "capacity"):
             # store the existing capacity as a variable
             existing_capacity = entry_key[0].capacity
             # convert entry_key[0] to string
             component_name_str = str(entry_key[0])
             # check if component_name_str is in capacities_df['Component']
-            if any(component_name_str in val for val in capacities_df['Component'].values):
+            if any(
+                component_name_str in val for val in capacities_df["Component"].values
+            ):
                 # update the existing capacity value in capacities_df
                 capacities_df.loc[
-                    capacities_df['Component'] == component_name_str, 'Existing Capacity'] = existing_capacity
+                    capacities_df["Component"] == component_name_str,
+                    "Existing Capacity",
+                ] = existing_capacity
         # check if the oemof object tuple has the 'expandable' attribute
-        if hasattr(entry_key[0], 'expandable'):
+        if hasattr(entry_key[0], "expandable"):
             # store the expandable boolean as a variable
             expandable = entry_key[0].expandable
             # convert entry_key[0] to string
             expandable_name_str = str(entry_key[0])
             # Check if expandable_name_str is in capacities_df['Component']
-            if any(expandable_name_str in val for val in capacities_df['Component'].values):
+            if any(
+                expandable_name_str in val for val in capacities_df["Component"].values
+            ):
                 # Update the existing expandable value in capacities_df
                 capacities_df.loc[
-                    capacities_df['Component'] == expandable_name_str, 'Optimizable'] = expandable
+                    capacities_df["Component"] == expandable_name_str, "Optimizable"
+                ] = expandable
         # check if the oemof object tuple has the 'capacity_potential' attribute
-        if hasattr(entry_key[0], 'capacity_potential'):
+        if hasattr(entry_key[0], "capacity_potential"):
             # store the capacity potential as a variable
             capacity_potential = entry_key[0].capacity_potential
             # convert entry_key[0] to string
             cp_name_str = str(entry_key[0])
             # Check if cp_name_str is in capacities_df['Component']
-            if any(cp_name_str in val for val in capacities_df['Component'].values):
+            if any(cp_name_str in val for val in capacities_df["Component"].values):
                 # Update the existing expandable value in capacities_df
                 capacities_df.loc[
-                    capacities_df['Component'] == cp_name_str, 'Capacity Potential'] = capacity_potential
+                    capacities_df["Component"] == cp_name_str, "Capacity Potential"
+                ] = capacity_potential
     return capacities_df
 
 
 def create_storage_capacities_table(all_scalars, results):
     # ToDo: this function requires the naming of storage components to have 'storage' in them, there is
     #  probably a cleaner way of doing it
     # ToDo: this is a bit of a repetition of the above function, maybe there is a better way to do this?
     # ToDo: note that for storages, storage capacity is the capacity in e.g. MWh and capacity is the
     #  max input/output in e.g. MW
     # set columns of the capacities dataframe
-    storage_capacities_df = pd.DataFrame(columns=['Component', 'Type', 'Carrier', 'Existing Storage Capacity',
-                                                  'Existing Max Input/Output', 'Storage Capacity Potential',
-                                                  'Max Input/Output Potential', 'Optimizable',
-                                                  'Optimized Storage Capacity', 'Optimized Max Input/Output'])
+    storage_capacities_df = pd.DataFrame(
+        columns=[
+            "Component",
+            "Type",
+            "Carrier",
+            "Existing Storage Capacity",
+            "Existing Max Input/Output",
+            "Storage Capacity Potential",
+            "Max Input/Output Potential",
+            "Optimizable",
+            "Optimized Storage Capacity",
+            "Optimized Max Input/Output",
+        ]
+    )
     # create an empty set for the component names
     component_names = set()
     # iterate over the index and row of the dataframe
     for idx, row in all_scalars.iterrows():
         # store variables to be included in the dataframe
         component_name = idx[0]
         component_variable = idx[1]
-        component_type = row['type']
-        component_carrier = row['carrier']
+        component_type = row["type"]
+        component_carrier = row["carrier"]
         # only include component names that haven't already been included to avoid repetition,
         # and only include component names that have 'storage' in
-        if component_name not in component_names and 'storage' in component_name:
+        if component_name not in component_names and "storage" in component_name:
             component_names.add(component_name)
             # add component name and corresponding type and carrier to the dataframe
-            storage_capacities_df = storage_capacities_df._append({'Component': component_name,
-                                                   'Type': component_type,
-                                                   'Carrier': component_carrier}, ignore_index=True)
+            storage_capacities_df = storage_capacities_df._append(
+                {
+                    "Component": component_name,
+                    "Type": component_type,
+                    "Carrier": component_carrier,
+                },
+                ignore_index=True,
+            )
         # check if 'invest' is equal to the component_variable
-        if 'invest' == component_variable:
+        if "invest" == component_variable:
             # if it is, get the corresponding 'var_value' for the optimized capacity value
-            component_opt_capacity = row['var_value']
+            component_opt_capacity = row["var_value"]
             # if the value is -0.0, adapt this to 0.0
             if component_opt_capacity == -0.0:
                 component_opt_capacity = 0.0
             # add or update 'Optimized Storage Capacity' for the component_name with the optimized capacity value
             storage_capacities_df.loc[
-                storage_capacities_df['Component'] == component_name,
-                'Optimized Storage Capacity'] = component_opt_capacity
+                storage_capacities_df["Component"] == component_name,
+                "Optimized Storage Capacity",
+            ] = component_opt_capacity
         # check if 'invest_out' is in the component_variable
-        if 'invest_out' in component_variable:
+        if "invest_out" in component_variable:
             # if it is, get the corresponding 'var_value' for the optimized capacity value
-            component_opt_capacity = row['var_value']
+            component_opt_capacity = row["var_value"]
             # if the value is -0.0, adapt this to 0.0
             if component_opt_capacity == -0.0:
                 component_opt_capacity = 0.0
             # add or update 'Optimized Max Input/Output' for the component_name with the optimized capacity value
             storage_capacities_df.loc[
-                storage_capacities_df['Component'] == component_name,
-                'Optimized Max Input/Output'] = component_opt_capacity
+                storage_capacities_df["Component"] == component_name,
+                "Optimized Max Input/Output",
+            ] = component_opt_capacity
 
     # loop through the results dict
     for entry_key, entry_value in results.items():
         # check if the oemof object tuple has the 'storage_capacity' attribute
-        if hasattr(entry_key[0], 'storage_capacity'):
+        if hasattr(entry_key[0], "storage_capacity"):
             # store the existing capacity as a variable
             existing_storage_capacity = entry_key[0].storage_capacity
             # convert entry_key[0] to string
             component_name_str = str(entry_key[0])
             # check if component_name_str is in storage_capacities_df['Component']
-            if any(component_name_str in val for val in storage_capacities_df['Component'].values):
+            if any(
+                component_name_str in val
+                for val in storage_capacities_df["Component"].values
+            ):
                 # update the existing capacity value in capacities_df
                 storage_capacities_df.loc[
-                    storage_capacities_df[
-                        'Component'] == component_name_str, 'Existing Storage Capacity'] = existing_storage_capacity
+                    storage_capacities_df["Component"] == component_name_str,
+                    "Existing Storage Capacity",
+                ] = existing_storage_capacity
         # check if the oemof object tuple has the 'capacity' attribute
-        if hasattr(entry_key[0], 'capacity'):
+        if hasattr(entry_key[0], "capacity"):
             # store the existing capacity as a variable
             existing_capacity = entry_key[0].capacity
             # convert entry_key[0] to string
             component_name_str = str(entry_key[0])
             # check if component_name_str is in storage_capacities_df['Component']
-            if any(component_name_str in val for val in storage_capacities_df['Component'].values):
+            if any(
+                component_name_str in val
+                for val in storage_capacities_df["Component"].values
+            ):
                 # update the existing capacity value in capacities_df
                 storage_capacities_df.loc[
-                    storage_capacities_df[
-                        'Component'] == component_name_str, 'Existing Max Input/Output'] = existing_capacity
+                    storage_capacities_df["Component"] == component_name_str,
+                    "Existing Max Input/Output",
+                ] = existing_capacity
         # check if the oemof object tuple has the 'expandable' attribute
-        if hasattr(entry_key[0], 'expandable'):
+        if hasattr(entry_key[0], "expandable"):
             # store the expandable boolean as a variable
             expandable = entry_key[0].expandable
             # convert entry_key[0] to string
             expandable_name_str = str(entry_key[0])
             # Check if expandable_name_str is in storage_capacities_df['Component']
-            if any(expandable_name_str in val for val in storage_capacities_df['Component'].values):
+            if any(
+                expandable_name_str in val
+                for val in storage_capacities_df["Component"].values
+            ):
                 # Update the existing expandable value in storage_capacities_df
                 storage_capacities_df.loc[
-                    storage_capacities_df['Component'] == expandable_name_str, 'Optimizable'] = expandable
+                    storage_capacities_df["Component"] == expandable_name_str,
+                    "Optimizable",
+                ] = expandable
         # check if the oemof object tuple has the 'storage_capacity_potential' attribute
-        if hasattr(entry_key[0], 'storage_capacity_potential'):
+        if hasattr(entry_key[0], "storage_capacity_potential"):
             # store the storage capacity potential as a variable
             storage_capacity_potential = entry_key[0].storage_capacity_potential
             # convert entry_key[0] to string
             cp_name_str = str(entry_key[0])
             # Check if cp_name_str is in storage_capacities_df['Component']
-            if any(cp_name_str in val for val in storage_capacities_df['Component'].values):
+            if any(
+                cp_name_str in val for val in storage_capacities_df["Component"].values
+            ):
                 # Update the existing expandable value in storage_capacities_df
                 storage_capacities_df.loc[
-                    storage_capacities_df['Component'] == cp_name_str, 'Storage Capacity Potential'] = storage_capacity_potential
+                    storage_capacities_df["Component"] == cp_name_str,
+                    "Storage Capacity Potential",
+                ] = storage_capacity_potential
         # check if the oemof object tuple has the 'capacity_potential' attribute
-        if hasattr(entry_key[0], 'capacity_potential'):
+        if hasattr(entry_key[0], "capacity_potential"):
             # store the capacity potential as a variable
             capacity_potential = entry_key[0].capacity_potential
             # convert entry_key[0] to string
             cp_name_str = str(entry_key[0])
             # Check if cp_name_str is in storage_capacities_df['Component']
-            if any(cp_name_str in val for val in storage_capacities_df['Component'].values):
+            if any(
+                cp_name_str in val for val in storage_capacities_df["Component"].values
+            ):
                 # Update the existing expandable value in storage_capacities_df
                 storage_capacities_df.loc[
-                    storage_capacities_df['Component'] == cp_name_str, 'Max Input/Output Potential'] = capacity_potential
+                    storage_capacities_df["Component"] == cp_name_str,
+                    "Max Input/Output Potential",
+                ] = capacity_potential
 
     return storage_capacities_df
 
 
 def create_aggregated_flows_table(aggregated_flows):
     # Create an empty DataFrame to store the flows
-    flows_df = pd.DataFrame(columns=['From', 'To', 'Aggregated Flow'])
+    flows_df = pd.DataFrame(columns=["From", "To", "Aggregated Flow"])
 
     # Iterate over the items of the Series
     for idx, value in aggregated_flows.items():
         # Extract the source, target, and var_name from the index
         from_, to, _ = idx
 
         # Append a row to the DataFrame
-        flows_df = flows_df._append({'From': from_, 'To': to, 'Aggregated Flow': float(value)}, ignore_index=True)
+        flows_df = flows_df._append(
+            {"From": from_, "To": to, "Aggregated Flow": float(value)},
+            ignore_index=True,
+        )
 
     return flows_df
 
 
 def create_costs_table(all_scalars, results):
     # create an empty dataframe
-    costs_df = pd.DataFrame(columns=['Component', 'Upfront Investment Cost',
-                                                  'Annuity (CAPEX + Fixed O&M)', 'Variable Costs (In)',
-                                                  'Variable Costs (Out)'])
+    costs_df = pd.DataFrame(
+        columns=[
+            "Component",
+            "Upfront Investment Cost",
+            "Annuity (CAPEX + Fixed O&M)",
+            "Variable Costs (In)",
+            "Variable Costs (Out)",
+        ]
+    )
     # create an empty set for the component names
     component_names = set()
     # iterate over the index and row of the dataframe
     for idx, row in all_scalars.iterrows():
         # store variables to be included in the dataframe
         component_name = idx[0]
         component_variable = idx[1]
         # only include component names that haven't already been included to avoid repetition,
         # and don't include system in the dataframe because this refers to the total system costs (include elsewhere)
         # and don't include the storage components because these are stored in a different table
-        if component_name not in component_names and component_name != 'system' and 'storage' not in component_name:
+        if (
+            component_name not in component_names
+            and component_name != "system"
+            and "storage" not in component_name
+        ):
             component_names.add(component_name)
             # add component name and corresponding type and carrier to the dataframe
-            costs_df = costs_df._append({'Component': component_name}, ignore_index=True)
+            costs_df = costs_df._append(
+                {"Component": component_name}, ignore_index=True
+            )
 
         # check if 'invest_costs_out' is in the component_variable
-        if 'invest_costs_out' in component_variable:
+        if "invest_costs_out" in component_variable:
             # if it is, get the corresponding 'var_value' for the investment cost value
-            invest_costs_out = row['var_value']
+            invest_costs_out = row["var_value"]
             # if the value is -0.0, adapt this to 0.0
             if invest_costs_out == -0.0:
                 invest_costs_out = 0.0
             # add or update 'Annuity (CAPEX + Fixed O&M)' for the component_name with the optimized capacity value
             costs_df.loc[
-                costs_df['Component'] == component_name, 'Annuity (CAPEX + Fixed O&M)'] = invest_costs_out
+                costs_df["Component"] == component_name, "Annuity (CAPEX + Fixed O&M)"
+            ] = invest_costs_out
         # check if 'variable_costs_in' is in the component_variable
-        if 'variable_costs_in' in component_variable:
+        if "variable_costs_in" in component_variable:
             # if it is, get the corresponding 'var_value' for the variable cost in value
-            variable_costs_in = row['var_value']
+            variable_costs_in = row["var_value"]
             # if the value is -0.0, adapt this to 0.0
             if variable_costs_in == -0.0:
                 variable_costs_in = 0.0
             # add or update 'Variable Costs (In)' for the component_name with the optimized capacity value
             costs_df.loc[
-                costs_df['Component'] == component_name, 'Variable Costs (In)'] = variable_costs_in
+                costs_df["Component"] == component_name, "Variable Costs (In)"
+            ] = variable_costs_in
         # check if 'variable_costs_out' is in the component_variable
-        if 'variable_costs_out' in component_variable:
+        if "variable_costs_out" in component_variable:
             # if it is, get the corresponding 'var_value' for the variable cost out value
-            variable_costs_out = row['var_value']
+            variable_costs_out = row["var_value"]
             # if the value is -0.0, adapt this to 0.0
             if variable_costs_out == -0.0:
                 variable_costs_out = 0.0
             # add or update 'Variable Costs (Out)' for the component_name with the optimized capacity value
             costs_df.loc[
-                costs_df['Component'] == component_name, 'Variable Costs (Out)'] = variable_costs_out
+                costs_df["Component"] == component_name, "Variable Costs (Out)"
+            ] = variable_costs_out
 
     return costs_df
 
 
 def post_processing(params, results, results_path):
     # initiate calculator for post-processing
     calculator = Calculator(params, results)
@@ -373,15 +463,17 @@
     # calculate scalars using functions from clc module
     aggregated_flows = clc.AggregatedFlows(calculator).result
     storage_losses = clc.StorageLosses(calculator).result
     transmission_losses = clc.TransmissionLosses(calculator).result
     invested_capacity = clc.InvestedCapacity(calculator).result
     invested_storage_capacity = clc.InvestedStorageCapacity(calculator).result
     invested_capacity_costs = clc.InvestedCapacityCosts(calculator).result
-    invested_storage_capacity_costs = clc.InvestedStorageCapacityCosts(calculator).result
+    invested_storage_capacity_costs = clc.InvestedStorageCapacityCosts(
+        calculator
+    ).result
     summed_carrier_costs = clc.SummedCarrierCosts(calculator).result
     summed_marginal_costs = clc.SummedMarginalCosts(calculator).result
     total_system_costs = clc.TotalSystemCosts(calculator).result
 
     # combine all results into a single dataframe
     all_scalars = [
         aggregated_flows,
@@ -398,67 +490,69 @@
     all_scalars = pd.concat(all_scalars, axis=0)
     all_scalars = naming.map_var_names(
         all_scalars,
         calculator.scalar_params,
         calculator.busses,
         calculator.links,
     )
-    all_scalars = naming.add_component_info(
-        all_scalars, calculator.scalar_params
-    )
-    print('Total System Cost', total_system_costs)
+    all_scalars = naming.add_component_info(all_scalars, calculator.scalar_params)
+    print("Total System Cost", total_system_costs)
     total_system_costs.index.names = ("name", "var_name")
     all_scalars = pd.concat([all_scalars, total_system_costs], axis=0)
     all_scalars = all_scalars.sort_values(by=["carrier", "tech", "var_name"])
     # save all scalar results to a csv file
-    filepath_name_all_scalars = os.path.join(results_path, 'all_scalars.csv')
+    filepath_name_all_scalars = os.path.join(results_path, "all_scalars.csv")
     all_scalars.to_csv(filepath_name_all_scalars)
 
     # saves all hourly timeseries as a dataframe (see test_postprocessing.py in oemof-tabular/tests
     # for example if wanting to filter particular nodes)
     all_sequences = clc.AggregatedFlows(calculator, resample_mode="H")
     # save all timeseries (sequence) results to a csv file
-    filepath_name_all_sequences = os.path.join(results_path, 'all_sequences.csv')
+    filepath_name_all_sequences = os.path.join(results_path, "all_sequences.csv")
     all_sequences.sequences.to_csv(filepath_name_all_sequences)
 
     capacities_df = create_capacities_table(all_scalars, results)
     storage_capacities_df = create_storage_capacities_table(all_scalars, results)
     flows_df = create_aggregated_flows_table(aggregated_flows)
     costs_df = create_costs_table(all_scalars, results)
 
     # store the relevant KPI variables
-    specific_system_cost = round(specific_system_costs(all_scalars, total_system_costs), 3)
+    specific_system_cost = round(
+        specific_system_costs(all_scalars, total_system_costs), 3
+    )
     renewable_share = calculate_renewable_share(results)
     excess_gen = excess_generation(all_scalars)
     total_emissions = calculate_total_emissions(results)
 
     # create a dataframe with the KPI variables
-    kpi_data = {'Variable': ['specific_system_cost', 'renewable_share', 'total_emissions'],
-                'Value': [specific_system_cost, renewable_share, total_emissions]}
+    kpi_data = {
+        "Variable": ["specific_system_cost", "renewable_share", "total_emissions"],
+        "Value": [specific_system_cost, renewable_share, total_emissions],
+    }
     # store KPI data as a dataframe
     kpi_df = pd.DataFrame(kpi_data)
     for key, value in excess_gen.items():
-        kpi_df = kpi_df._append({'Variable': key, 'Value': value}, ignore_index=True)
+        kpi_df = kpi_df._append({"Variable": key, "Value": value}, ignore_index=True)
         # replace any parameters with '-' in the name with '_' for uniformity
-        kpi_df['Variable'] = kpi_df['Variable'].str.replace('-', '_')
+        kpi_df["Variable"] = kpi_df["Variable"].str.replace("-", "_")
     # save all KPI results to a csv file
-    filepath_name_kpis = os.path.join(results_path, 'kpis.csv')
+    filepath_name_kpis = os.path.join(results_path, "kpis.csv")
     # save the DataFrame to a CSV file
     kpi_df.to_csv(filepath_name_kpis, index=False)
     # save all capacities to a csv file
-    filepath_name_capacities = os.path.join(results_path, 'capacities.csv')
+    filepath_name_capacities = os.path.join(results_path, "capacities.csv")
     # save the DataFrame to a CSV file
     capacities_df.to_csv(filepath_name_capacities, index=False)
     # save all storage capacities to a csv file
-    filepath_name_stor_capacities = os.path.join(results_path, 'storage_capacities.csv')
+    filepath_name_stor_capacities = os.path.join(results_path, "storage_capacities.csv")
     # save the DataFrame to a CSV file
     storage_capacities_df.to_csv(filepath_name_stor_capacities, index=False)
     # save all flows to a csv file
-    filepath_name_flows = os.path.join(results_path, 'flows.csv')
+    filepath_name_flows = os.path.join(results_path, "flows.csv")
     # save the DataFrame to a CSV file
     flows_df.to_csv(filepath_name_flows, index=False)
     # save all costs to a csv file
-    filepath_name_costs = os.path.join(results_path, 'costs.csv')
+    filepath_name_costs = os.path.join(results_path, "costs.csv")
     # save the DataFrame to a CSV file
     costs_df.to_csv(filepath_name_costs, index=False)
 
     return all_scalars
```

### Comparing `oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins/wefe/facades/pv_panel.py` & `oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins/wefe/facades/pv_panel.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
         Cell temperature at reference conditions. Default: 25
     noct: numeric
         Normal operating cell temperature. Default: 48
 
     SHOULD INCLUDE FUNCTIONS AND EXAMPLE HERE
 
     """
+
     from_bus: Bus
 
     to_bus: Bus
 
     carrier: str
 
     tech: str
@@ -114,15 +115,17 @@
         # raise error if air temperature list and solar irradiance list are different lengths
         if len(t_air_values) != len(ghi_values):
             raise ValueError("Length mismatch between t_air and ghi profiles.")
         # calculates the temperature factor values
         pv_tf_values = []
         for t_air, ghi in zip(t_air_values, ghi_values):
             t_c = t_air + ((self.noct - 20) / 800) * ghi
-            pv_tf = self.p_rpv * (1 / self.r_ref) * (1 + self.n_t * (t_c - self.t_c_ref))
+            pv_tf = (
+                self.p_rpv * (1 / self.r_ref) * (1 + self.n_t * (t_c - self.t_c_ref))
+            )
             pv_tf_values.append(pv_tf)
 
         self.conversion_factors.update(
             {
                 self.from_bus: sequence(1),
                 self.to_bus: sequence(pv_tf_values),
             }
```

### Comparing `oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins.egg-info/PKG-INFO` & `oemof_tabular_plugins-0.0.2rc1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oemof-tabular-plugins
-Version: 0.0.1rc3
+Version: 0.0.2rc1
 Summary: A package that contains various constraint facades to be used with oemof-tabular
 Author-email: Ciara Dunks <ciara.dunks@rl-institut.de>, Pierre-François Duc <pierre-francois.duc@rl-institut.de>
 Project-URL: Homepage, https://github.com/rl-institut/oemof-tabular-plugins
 Project-URL: Issues, https://github.com/rl-institut/oemof-tabular-plugins/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -29,19 +29,19 @@
    :widths: auto
 
    * - License
      - |badge_license|
    * - Documentation
      - |badge_documentation|
    * - Publication
-     - 
+     -
    * - Development
-     - |badge_issue_open| |badge_issue_closes| |badge_pr_open| |badge_pr_closes|
+     - |badge_issue_open| |badge_issue_closes| |badge_pr_open| |badge_pr_closes| |badge_black|
    * - Community
-     - |badge_contributing| |badge_contributors| |badge_repo_counts|
+     - |badge_contributing| |badge_contributors|
 
 .. contents::
     :depth: 2
     :local:
     :backlinks: top
 
 Introduction
@@ -83,24 +83,25 @@
 .. |badge_documentation| image:: https://img.shields.io/github/actions/workflow/status/rl-institut/super-repo/gh-pages.yml?branch=production
     :target: https://rl-institut.github.io/super-repo/
     :alt: Documentation
 
 .. |badge_contributing| image:: https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat
     :alt: contributions
 
-.. |badge_repo_counts| image:: http://hits.dwyl.com/rl-institut/super-repo.svg
-    :alt: counter
-
 .. |badge_contributors| image:: https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square
     :alt: contributors
 
 .. |badge_issue_open| image:: https://img.shields.io/github/issues-raw/rl-institut/super-repo
     :alt: open issues
 
 .. |badge_issue_closes| image:: https://img.shields.io/github/issues-closed-raw/rl-institut/super-repo
     :alt: closes issues
 
 .. |badge_pr_open| image:: https://img.shields.io/github/issues-pr-raw/rl-institut/super-repo
-    :alt: closes issues
+    :alt: open pull requests
 
 .. |badge_pr_closes| image:: https://img.shields.io/github/issues-pr-closed-raw/rl-institut/super-repo
-    :alt: closes issues
+    :alt: closes pull requests
+
+.. |badge_black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: black linting badge
```

### Comparing `oemof-tabular-plugins-0.0.1rc3/src/oemof_tabular_plugins.egg-info/SOURCES.txt` & `oemof_tabular_plugins-0.0.2rc1/src/oemof_tabular_plugins.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,19 +6,23 @@
 src/oemof_tabular_plugins/_version.py
 src/oemof_tabular_plugins.egg-info/PKG-INFO
 src/oemof_tabular_plugins.egg-info/SOURCES.txt
 src/oemof_tabular_plugins.egg-info/dependency_links.txt
 src/oemof_tabular_plugins.egg-info/entry_points.txt
 src/oemof_tabular_plugins.egg-info/requires.txt
 src/oemof_tabular_plugins.egg-info/top_level.txt
+src/oemof_tabular_plugins/datapackage/__init__.py
+src/oemof_tabular_plugins/datapackage/building.py
 src/oemof_tabular_plugins/general/__init__.py
 src/oemof_tabular_plugins/general/constraint_facades.py
 src/oemof_tabular_plugins/general/constraints.py
 src/oemof_tabular_plugins/general/post_processing.py
+src/oemof_tabular_plugins/general/post_processing_moo.py
 src/oemof_tabular_plugins/general/pre_processing.py
+src/oemof_tabular_plugins/general/pre_processing_moo.py
 src/oemof_tabular_plugins/hydrogen/__init__.py
 src/oemof_tabular_plugins/hydrogen/constraint_facades.py
 src/oemof_tabular_plugins/hydrogen/constraints.py
 src/oemof_tabular_plugins/hydrogen/post_processing.py
 src/oemof_tabular_plugins/wefe/__init__.py
 src/oemof_tabular_plugins/wefe/constraint_facades.py
 src/oemof_tabular_plugins/wefe/constraints.py
```

