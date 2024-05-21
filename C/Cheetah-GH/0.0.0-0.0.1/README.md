# Comparing `tmp/cheetah_gh-0.0.0.tar.gz` & `tmp/cheetah_gh-0.0.1.tar.gz`

## Comparing `cheetah_gh-0.0.0.tar` & `cheetah_gh-0.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 cheetah_gh-0.0.0/.gitattributes
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cheetah_gh-0.0.0/src/cheetah_GH/__init__.py
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 cheetah_gh-0.0.0/src/cheetah_GH/gh_and_py_runner.py
--rw-r--r--   0        0        0     9293 2020-02-02 00:00:00.000000 cheetah_gh-0.0.0/src/cheetah_GH/helpers.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 cheetah_gh-0.0.0/src/cheetah_GH/unittest_runner.py
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 cheetah_gh-0.0.0/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cheetah_gh-0.0.0/LICENSE.md
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 cheetah_gh-0.0.0/README.md
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 cheetah_gh-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 cheetah_gh-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 cheetah_gh-0.0.1/.gitattributes
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cheetah_gh-0.0.1/src/Cheetah_GH/__init__.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 cheetah_gh-0.0.1/src/Cheetah_GH/gh_and_py_runner.py
+-rw-r--r--   0        0        0     9293 2020-02-02 00:00:00.000000 cheetah_gh-0.0.1/src/Cheetah_GH/helpers.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 cheetah_gh-0.0.1/src/Cheetah_GH/unittest_runner.py
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 cheetah_gh-0.0.1/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cheetah_gh-0.0.1/LICENSE.md
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 cheetah_gh-0.0.1/README.md
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 cheetah_gh-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 cheetah_gh-0.0.1/PKG-INFO
```

### Comparing `cheetah_gh-0.0.0/src/cheetah_GH/gh_and_py_runner.py` & `cheetah_gh-0.0.1/src/Cheetah_GH/gh_and_py_runner.py`

 * *Files identical despite different names*

### Comparing `cheetah_gh-0.0.0/src/cheetah_GH/helpers.py` & `cheetah_gh-0.0.1/src/Cheetah_GH/helpers.py`

 * *Files identical despite different names*

### Comparing `cheetah_gh-0.0.0/src/cheetah_GH/unittest_runner.py` & `cheetah_gh-0.0.1/src/Cheetah_GH/unittest_runner.py`

 * *Files identical despite different names*

### Comparing `cheetah_gh-0.0.0/.gitignore` & `cheetah_gh-0.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cheetah_gh-0.0.0/PKG-INFO` & `cheetah_gh-0.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.3
-Name: cheetah_GH
-Version: 0.0.0
+Name: Cheetah_GH
+Version: 0.0.1
 Summary: Runs Grasshopper components and stops Rhino from Python components. Optionally runs Rhino3D and Grasshopper from the command line.
+Project-URL: Homepage, https://github.com/JamesParrott/Cheetah_GH
+Project-URL: Bug Tracker, https://github.com/JamesParrott/Cheetah_GH/issues
 Author-email: James Parrott <james.parrott@proton.me>
 License-File: LICENSE.md
 Keywords: Grasshopper,Rhino,components,control,runner,tests
 Classifier: Programming Language :: Python
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
```

