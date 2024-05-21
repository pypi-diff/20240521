# Comparing `tmp/cheetah_gh-0.1.3.tar.gz` & `tmp/cheetah_gh-0.1.4.tar.gz`

## Comparing `cheetah_gh-0.1.3.tar` & `cheetah_gh-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 cheetah_gh-0.1.3/.gitattributes
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 cheetah_gh-0.1.3/src/Cheetah_GH/__init__.py
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 cheetah_gh-0.1.3/src/Cheetah_GH/gh_and_py_runner.py
--rw-r--r--   0        0        0     9294 2020-02-02 00:00:00.000000 cheetah_gh-0.1.3/src/Cheetah_GH/helpers.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 cheetah_gh-0.1.3/src/Cheetah_GH/unittest_runner.py
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 cheetah_gh-0.1.3/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cheetah_gh-0.1.3/LICENSE.md
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 cheetah_gh-0.1.3/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 cheetah_gh-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 cheetah_gh-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 cheetah_gh-0.1.4/.gitattributes
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 cheetah_gh-0.1.4/src/Cheetah_GH/__init__.py
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 cheetah_gh-0.1.4/src/Cheetah_GH/gh_and_py_runner.py
+-rw-r--r--   0        0        0     9295 2020-02-02 00:00:00.000000 cheetah_gh-0.1.4/src/Cheetah_GH/helpers.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 cheetah_gh-0.1.4/src/Cheetah_GH/unittest_runner.py
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 cheetah_gh-0.1.4/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cheetah_gh-0.1.4/LICENSE.md
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 cheetah_gh-0.1.4/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 cheetah_gh-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 cheetah_gh-0.1.4/PKG-INFO
```

### Comparing `cheetah_gh-0.1.3/src/Cheetah_GH/gh_and_py_runner.py` & `cheetah_gh-0.1.4/src/Cheetah_GH/gh_and_py_runner.py`

 * *Files identical despite different names*

### Comparing `cheetah_gh-0.1.3/src/Cheetah_GH/helpers.py` & `cheetah_gh-0.1.4/src/Cheetah_GH/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
     x = pos[0] + (h % row_width)
     y = pos[1] + 220 * (h // row_width)
     return x, y
 
 def add_instance_of_userobject_to_canvas(
     name,
     plugin_files,
-    plug
+    plug,
     comp_number=1,
     pos = (200, 550),
     ):
     
     
     file_obj = next((v
                      for k, v in plugin_files.items()
```

### Comparing `cheetah_gh-0.1.3/src/Cheetah_GH/unittest_runner.py` & `cheetah_gh-0.1.4/src/Cheetah_GH/unittest_runner.py`

 * *Files identical despite different names*

### Comparing `cheetah_gh-0.1.3/.gitignore` & `cheetah_gh-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `cheetah_gh-0.1.3/pyproject.toml` & `cheetah_gh-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 
 
 
 [project]
 name = "Cheetah_GH"
-version = "0.1.3"
+version = "0.1.4"
 authors = [{name = "James Parrott", email = "james.parrott@proton.me"}]
 description = "Runs Grasshopper components and stops Rhino from Python components. Optionally runs Rhino3D and Grasshopper from the command line."
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=2.7"
 keywords = ["Rhino", "Grasshopper", "control", "components", "runner", "tests"]
 license = {file = "LICENSE.md"}
 classifiers = [
```

### Comparing `cheetah_gh-0.1.3/PKG-INFO` & `cheetah_gh-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: Cheetah_GH
-Version: 0.1.3
+Version: 0.1.4
 Summary: Runs Grasshopper components and stops Rhino from Python components. Optionally runs Rhino3D and Grasshopper from the command line.
 Project-URL: Homepage, https://github.com/JamesParrott/Cheetah_GH
 Project-URL: Bug Tracker, https://github.com/JamesParrott/Cheetah_GH/issues
 Author-email: James Parrott <james.parrott@proton.me>
 License-File: LICENSE.md
 Keywords: Grasshopper,Rhino,components,control,runner,tests
 Classifier: Programming Language :: Python
```

