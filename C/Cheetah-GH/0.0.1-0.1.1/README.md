# Comparing `tmp/cheetah_gh-0.0.1.tar.gz` & `tmp/cheetah_gh-0.1.1.tar.gz`

## Comparing `cheetah_gh-0.0.1.tar` & `cheetah_gh-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 cheetah_gh-0.0.1/.gitattributes
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cheetah_gh-0.0.1/src/Cheetah_GH/__init__.py
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 cheetah_gh-0.0.1/src/Cheetah_GH/gh_and_py_runner.py
--rw-r--r--   0        0        0     9293 2020-02-02 00:00:00.000000 cheetah_gh-0.0.1/src/Cheetah_GH/helpers.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 cheetah_gh-0.0.1/src/Cheetah_GH/unittest_runner.py
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 cheetah_gh-0.0.1/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cheetah_gh-0.0.1/LICENSE.md
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 cheetah_gh-0.0.1/README.md
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 cheetah_gh-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 cheetah_gh-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 cheetah_gh-0.1.1/.gitattributes
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 cheetah_gh-0.1.1/src/Cheetah_GH/__init__.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 cheetah_gh-0.1.1/src/Cheetah_GH/gh_and_py_runner.py
+-rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 cheetah_gh-0.1.1/src/Cheetah_GH/helpers.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 cheetah_gh-0.1.1/src/Cheetah_GH/unittest_runner.py
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 cheetah_gh-0.1.1/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cheetah_gh-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 cheetah_gh-0.1.1/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 cheetah_gh-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 cheetah_gh-0.1.1/PKG-INFO
```

### Comparing `cheetah_gh-0.0.1/src/Cheetah_GH/gh_and_py_runner.py` & `cheetah_gh-0.1.1/src/Cheetah_GH/gh_and_py_runner.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,54 +27,68 @@
 
 
 def start_UDP_server():
     HOST, PORT = "127.0.0.1", 9999
     with socketserver.UDPServer((HOST, PORT), MyUDPHandler) as server:
         server.serve_forever()
 
-
-if __name__ == '__main__':
+def run_GH_file(gh_file, extra_env_vars):
     p = multiprocessing.Process(target=start_UDP_server)
     p.daemon = True
     print('Starting output printing UDP server.  Press Ctrl+C to quit.')
     p.start()
 
 
-    gh_file_path = sys.argv[1]
 
     env = os.environ.copy()
 
     # By default, exit Rhino afterwards.
     env['CHEETAH_GH_NON_INTERACTIVE'] = 'True'
 
 
-    # Subsequent trailing command line args are env variable names and values.
-    other_args = iter(sys.argv[2:])
-    env.update(zip(other_args, other_args))
+    env.update()
 
     
     
 
-    print(rf'Opening: {gh_file_path}')
+    print(rf'Opening: {gh_file}')
 
     result = subprocess.run(
          ( r'"C:\Program Files\Rhino 8\System\Rhino.exe" /nosplash /runscript='
-          rf'"-_grasshopper _editor _load _document _open {gh_file_path} '
+          rf'"-_grasshopper _editor _load _document _open {gh_file} '
            r'_enter _exit _enterend"'
          )
         ,env = env
         )
     p.terminate()
 
-    print(f'{result.returncode=}')
-    print(f'{p.exitcode=}')
+    return result, p.exitcode
+
+
+
+
+def main(args = sys.argv[1:]):
 
 
-    if result.returncode != 0 or p.exitcode: 
+    gh_file = args[0]
+    
+    # Subsequent trailing command line args are env variable names and values.
+    other_args = iter(args[1:])
+
+    extra_env_vars = dict(zip(other_args, other_args))
+
+    result, exitcode = run_GH_file(gh_file = gh_file, extra_env_vars = extra_env_vars)
+
+    print(f'{result.returncode=}')
+    print(f'{exitcode=}')
+
+    if result.returncode != 0 or exitcode: 
         raise Exception(
-             'Some tests were failed (or an error occurred during testing). \n'
+             'An error occurred while running: {gh_file}. \n'
             f'Test runner retcode: {result.returncode}\n'
-            f'Test output server exitcode: {p.exitcode}\n'
+            f'Test output server exitcode: {exitcode}\n'
             )
+    return 0
 
 
-    sys.exit(0)
+if __name__ == '__main__':
+    sys.exit(main())
```

### Comparing `cheetah_gh-0.0.1/src/Cheetah_GH/helpers.py` & `cheetah_gh-0.1.1/src/Cheetah_GH/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,17 @@
 import Rhino.NodeInCode.Components
 import Grasshopper
 import rhinoscriptsyntax as rs
 
 
 TMP = tempfile.gettempdir()
 
-DIR = TMP
+DIR = os.path.join(TMP, 'Cheetah_GH')
 
-for SUB_DIR in ( 'sDNA_GH', 'tests'):
-    DIR = os.path.join(DIR, SUB_DIR)
-    if not os.path.isdir(DIR):
-        os.mkdir(DIR)
+os.makedirs(DIR)
 
 try:
     ghdoc
 except NameError:
     import scriptcontext as sc
 
     if sc.doc == Rhino.RhinoDoc.ActiveDoc:
@@ -155,20 +152,20 @@
     h = comp_number * row_height
     x = pos[0] + (h % row_width)
     y = pos[1] + 220 * (h // row_width)
     return x, y
 
 def add_instance_of_userobject_to_canvas(
     name,
-    plugin_files = None,
+    plugin_files,
+    plug
     comp_number=1,
     pos = (200, 550),
     ):
     
-    plugin_files = plugin_files or get_plugin_files('sDNA_GH')
     
     file_obj = next((v
                      for k, v in plugin_files.items() 
                      if name.lower() in k.lower()
                     )
                     ,None)
                     
@@ -266,31 +263,35 @@
     def flush(self):
         pass
 
 
 
 
 
-def save_doc_to_(name = 'tmp_sDNA_GH_api_tests_working_file.3dm', dir_ = DIR):
+def save_doc_to_(name, dir_ = None):
     # 'Dale Fugier'
     # https://discourse.mcneel.com/t/sys-exit-shows-popup-window-instead-of-just-exiting/163811/7
 
+    dir_ = dir_ or DIR
+
     path = os.path.join(dir_, name) if dir_ else name
     rs.Command('_-SaveAs ' + path, True)
     
 
 
 
 
 
-def exit_Rhino():
+def exit_Rhino(save_3dm_to = None, save_to_dir = None):
     #'Dale Fugier'
     # https://discourse.mcneel.com/t/sys-exit-shows-popup-window-instead-of-just-exiting/163811/7
 
-    save_doc_to_()
+    if save_3dm_to:
+        save_doc_to_(name = save_3dm_to, dir_ = save_to_dir)
+
     Rhino.RhinoDoc.ActiveDoc.Modified = False
 
     hWnd = Rhino.RhinoApp.MainWindowHandle()
     ctypes.windll.user32.PostMessageW(hWnd, 0x0010, 0, 0) # - quits but doesn't set return code
     # ctypes.windll.user32.PostQuitMessage(ret_code) # - doesn't quit, even if Rhino doc saved.
     # ctypes.windll.user32.PostMessageW(hWnd, 0x0010, ret_code, 0) # - quits but doesn't set return code
     # ctypes.windll.user32.PostMessageW(hWnd, 0x0012, ret_code, 0) # - makes Rhino hang. ret code 1 is set
```

### Comparing `cheetah_gh-0.0.1/src/Cheetah_GH/unittest_runner.py` & `cheetah_gh-0.1.1/src/Cheetah_GH/unittest_runner.py`

 * *Files identical despite different names*

### Comparing `cheetah_gh-0.0.1/.gitignore` & `cheetah_gh-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cheetah_gh-0.0.1/pyproject.toml` & `cheetah_gh-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 build-backend = "hatchling.build"
 
 
 
 
 [project]
 name = "Cheetah_GH"
-version = "0.0.1"
+version = "0.1.1"
 authors = [{name = "James Parrott", email = "james.parrott@proton.me"}]
 description = "Runs Grasshopper components and stops Rhino from Python components. Optionally runs Rhino3D and Grasshopper from the command line."
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=2.7"
 keywords = ["Rhino", "Grasshopper", "control", "components", "runner", "tests"]
 license = {file = "LICENSE.md"}
 classifiers = [
     "Programming Language :: Python",
 ]
 dependencies = []
 
+[project.scripts]
+Cheetah_GH="Cheetah_GH.gh_and_py_runner:main"
 
 [project.urls]   
 "Homepage" = "https://github.com/JamesParrott/Cheetah_GH"
 "Bug Tracker" = "https://github.com/JamesParrott/Cheetah_GH/issues"
```

### Comparing `cheetah_gh-0.0.1/PKG-INFO` & `cheetah_gh-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: Cheetah_GH
-Version: 0.0.1
+Version: 0.1.1
 Summary: Runs Grasshopper components and stops Rhino from Python components. Optionally runs Rhino3D and Grasshopper from the command line.
 Project-URL: Homepage, https://github.com/JamesParrott/Cheetah_GH
 Project-URL: Bug Tracker, https://github.com/JamesParrott/Cheetah_GH/issues
 Author-email: James Parrott <james.parrott@proton.me>
 License-File: LICENSE.md
 Keywords: Grasshopper,Rhino,components,control,runner,tests
 Classifier: Programming Language :: Python
```

