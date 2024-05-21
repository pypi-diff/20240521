# Comparing `tmp/cheetah_gh-0.1.2.tar.gz` & `tmp/cheetah_gh-0.1.3.tar.gz`

## Comparing `cheetah_gh-0.1.2.tar` & `cheetah_gh-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 cheetah_gh-0.1.2/.gitattributes
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 cheetah_gh-0.1.2/src/Cheetah_GH/__init__.py
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 cheetah_gh-0.1.2/src/Cheetah_GH/gh_and_py_runner.py
--rw-r--r--   0        0        0     9294 2020-02-02 00:00:00.000000 cheetah_gh-0.1.2/src/Cheetah_GH/helpers.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 cheetah_gh-0.1.2/src/Cheetah_GH/unittest_runner.py
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 cheetah_gh-0.1.2/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cheetah_gh-0.1.2/LICENSE.md
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 cheetah_gh-0.1.2/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 cheetah_gh-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 cheetah_gh-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 cheetah_gh-0.1.3/.gitattributes
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 cheetah_gh-0.1.3/src/Cheetah_GH/__init__.py
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 cheetah_gh-0.1.3/src/Cheetah_GH/gh_and_py_runner.py
+-rw-r--r--   0        0        0     9294 2020-02-02 00:00:00.000000 cheetah_gh-0.1.3/src/Cheetah_GH/helpers.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 cheetah_gh-0.1.3/src/Cheetah_GH/unittest_runner.py
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 cheetah_gh-0.1.3/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cheetah_gh-0.1.3/LICENSE.md
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 cheetah_gh-0.1.3/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 cheetah_gh-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 cheetah_gh-0.1.3/PKG-INFO
```

### Comparing `cheetah_gh-0.1.2/src/Cheetah_GH/gh_and_py_runner.py` & `cheetah_gh-0.1.3/src/Cheetah_GH/gh_and_py_runner.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,26 +43,28 @@
 
     # By default, exit Rhino afterwards.
     env['CHEETAH_GH_NON_INTERACTIVE'] = 'True'
 
 
     env.update(extra_env_vars)
 
-    
-    
 
     print(rf'Opening: {gh_file}')
 
-    result = subprocess.run(
-         ( r'"C:\Program Files\Rhino 8\System\Rhino.exe" /nosplash /runscript='
+    command = ( 
+           r'"C:\Program Files\Rhino 8\System\Rhino.exe" /nosplash /runscript='
           rf'"-_grasshopper _editor _load _document _open {gh_file} '
-           r'_enter _exit _enterend"'
-         )
-        ,env = env
-        )
+          )
+
+    if env['CHEETAH_GH_NON_INTERACTIVE'].lower() not in ('', '0', 'false'):
+        command += ' _enter _exit'
+    command += ' _enterend"'
+
+    result = subprocess.run(command, env=env, shell=True)
+    
     p.terminate()
 
     return result, p.exitcode
```

### Comparing `cheetah_gh-0.1.2/src/Cheetah_GH/helpers.py` & `cheetah_gh-0.1.3/src/Cheetah_GH/helpers.py`

 * *Files identical despite different names*

### Comparing `cheetah_gh-0.1.2/src/Cheetah_GH/unittest_runner.py` & `cheetah_gh-0.1.3/src/Cheetah_GH/unittest_runner.py`

 * *Files identical despite different names*

### Comparing `cheetah_gh-0.1.2/.gitignore` & `cheetah_gh-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `cheetah_gh-0.1.2/pyproject.toml` & `cheetah_gh-0.1.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 
 
 
 [project]
 name = "Cheetah_GH"
-version = "0.1.2"
+version = "0.1.3"
 authors = [{name = "James Parrott", email = "james.parrott@proton.me"}]
 description = "Runs Grasshopper components and stops Rhino from Python components. Optionally runs Rhino3D and Grasshopper from the command line."
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=2.7"
 keywords = ["Rhino", "Grasshopper", "control", "components", "runner", "tests"]
 license = {file = "LICENSE.md"}
 classifiers = [
```

### Comparing `cheetah_gh-0.1.2/PKG-INFO` & `cheetah_gh-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: Cheetah_GH
-Version: 0.1.2
+Version: 0.1.3
 Summary: Runs Grasshopper components and stops Rhino from Python components. Optionally runs Rhino3D and Grasshopper from the command line.
 Project-URL: Homepage, https://github.com/JamesParrott/Cheetah_GH
 Project-URL: Bug Tracker, https://github.com/JamesParrott/Cheetah_GH/issues
 Author-email: James Parrott <james.parrott@proton.me>
 License-File: LICENSE.md
 Keywords: Grasshopper,Rhino,components,control,runner,tests
 Classifier: Programming Language :: Python
```

