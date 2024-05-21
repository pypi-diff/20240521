# Comparing `tmp/cheetah_gh-0.1.1.tar.gz` & `tmp/cheetah_gh-0.1.2.tar.gz`

## Comparing `cheetah_gh-0.1.1.tar` & `cheetah_gh-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 cheetah_gh-0.1.1/.gitattributes
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 cheetah_gh-0.1.1/src/Cheetah_GH/__init__.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 cheetah_gh-0.1.1/src/Cheetah_GH/gh_and_py_runner.py
--rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 cheetah_gh-0.1.1/src/Cheetah_GH/helpers.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 cheetah_gh-0.1.1/src/Cheetah_GH/unittest_runner.py
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 cheetah_gh-0.1.1/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cheetah_gh-0.1.1/LICENSE.md
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 cheetah_gh-0.1.1/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 cheetah_gh-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 cheetah_gh-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 cheetah_gh-0.1.2/.gitattributes
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 cheetah_gh-0.1.2/src/Cheetah_GH/__init__.py
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 cheetah_gh-0.1.2/src/Cheetah_GH/gh_and_py_runner.py
+-rw-r--r--   0        0        0     9294 2020-02-02 00:00:00.000000 cheetah_gh-0.1.2/src/Cheetah_GH/helpers.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 cheetah_gh-0.1.2/src/Cheetah_GH/unittest_runner.py
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 cheetah_gh-0.1.2/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cheetah_gh-0.1.2/LICENSE.md
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 cheetah_gh-0.1.2/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 cheetah_gh-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 cheetah_gh-0.1.2/PKG-INFO
```

### Comparing `cheetah_gh-0.1.1/src/Cheetah_GH/gh_and_py_runner.py` & `cheetah_gh-0.1.2/src/Cheetah_GH/gh_and_py_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     env = os.environ.copy()
 
     # By default, exit Rhino afterwards.
     env['CHEETAH_GH_NON_INTERACTIVE'] = 'True'
 
 
-    env.update()
+    env.update(extra_env_vars)
 
     
     
 
     print(rf'Opening: {gh_file}')
 
     result = subprocess.run(
```

### Comparing `cheetah_gh-0.1.1/src/Cheetah_GH/helpers.py` & `cheetah_gh-0.1.2/src/Cheetah_GH/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,14 +287,16 @@
 
     if save_3dm_to:
         save_doc_to_(name = save_3dm_to, dir_ = save_to_dir)
 
     Rhino.RhinoDoc.ActiveDoc.Modified = False
 
     hWnd = Rhino.RhinoApp.MainWindowHandle()
+
+    # TODO:  Fix.  Doesn't skip save file screen anymore.
     ctypes.windll.user32.PostMessageW(hWnd, 0x0010, 0, 0) # - quits but doesn't set return code
     # ctypes.windll.user32.PostQuitMessage(ret_code) # - doesn't quit, even if Rhino doc saved.
     # ctypes.windll.user32.PostMessageW(hWnd, 0x0010, ret_code, 0) # - quits but doesn't set return code
     # ctypes.windll.user32.PostMessageW(hWnd, 0x0012, ret_code, 0) # - makes Rhino hang. ret code 1 is set
     #                                                              # after killing it from Task Manager.
```

### Comparing `cheetah_gh-0.1.1/src/Cheetah_GH/unittest_runner.py` & `cheetah_gh-0.1.2/src/Cheetah_GH/unittest_runner.py`

 * *Files identical despite different names*

### Comparing `cheetah_gh-0.1.1/.gitignore` & `cheetah_gh-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `cheetah_gh-0.1.1/pyproject.toml` & `cheetah_gh-0.1.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 
 
 
 [project]
 name = "Cheetah_GH"
-version = "0.1.1"
+version = "0.1.2"
 authors = [{name = "James Parrott", email = "james.parrott@proton.me"}]
 description = "Runs Grasshopper components and stops Rhino from Python components. Optionally runs Rhino3D and Grasshopper from the command line."
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=2.7"
 keywords = ["Rhino", "Grasshopper", "control", "components", "runner", "tests"]
 license = {file = "LICENSE.md"}
 classifiers = [
```

### Comparing `cheetah_gh-0.1.1/PKG-INFO` & `cheetah_gh-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: Cheetah_GH
-Version: 0.1.1
+Version: 0.1.2
 Summary: Runs Grasshopper components and stops Rhino from Python components. Optionally runs Rhino3D and Grasshopper from the command line.
 Project-URL: Homepage, https://github.com/JamesParrott/Cheetah_GH
 Project-URL: Bug Tracker, https://github.com/JamesParrott/Cheetah_GH/issues
 Author-email: James Parrott <james.parrott@proton.me>
 License-File: LICENSE.md
 Keywords: Grasshopper,Rhino,components,control,runner,tests
 Classifier: Programming Language :: Python
```

