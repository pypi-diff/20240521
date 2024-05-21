# Comparing `tmp/cheetah_gh-0.1.4.tar.gz` & `tmp/cheetah_gh-0.1.5.tar.gz`

## Comparing `cheetah_gh-0.1.4.tar` & `cheetah_gh-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 cheetah_gh-0.1.4/.gitattributes
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 cheetah_gh-0.1.4/src/Cheetah_GH/__init__.py
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 cheetah_gh-0.1.4/src/Cheetah_GH/gh_and_py_runner.py
--rw-r--r--   0        0        0     9295 2020-02-02 00:00:00.000000 cheetah_gh-0.1.4/src/Cheetah_GH/helpers.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 cheetah_gh-0.1.4/src/Cheetah_GH/unittest_runner.py
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 cheetah_gh-0.1.4/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cheetah_gh-0.1.4/LICENSE.md
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 cheetah_gh-0.1.4/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 cheetah_gh-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 cheetah_gh-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 cheetah_gh-0.1.5/.gitattributes
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 cheetah_gh-0.1.5/src/Cheetah_GH/__init__.py
+-rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 cheetah_gh-0.1.5/src/Cheetah_GH/gh_and_py_runner.py
+-rw-r--r--   0        0        0     9295 2020-02-02 00:00:00.000000 cheetah_gh-0.1.5/src/Cheetah_GH/helpers.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 cheetah_gh-0.1.5/src/Cheetah_GH/unittest_runner.py
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 cheetah_gh-0.1.5/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cheetah_gh-0.1.5/LICENSE.md
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 cheetah_gh-0.1.5/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 cheetah_gh-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 cheetah_gh-0.1.5/PKG-INFO
```

### Comparing `cheetah_gh-0.1.4/src/Cheetah_GH/gh_and_py_runner.py` & `cheetah_gh-0.1.5/src/Cheetah_GH/gh_and_py_runner.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,40 +2,48 @@
 # -*- coding: utf-8 -*-
 # This test launcher script requires Python >=3.8 and an installation of Rhino 8.
 
 
 
 import os
 import sys
-import socketserver
-import multiprocessing
 import subprocess
 
 
 
 
-class MyUDPHandler(socketserver.BaseRequestHandler):
 
-    quit_on = 'TESTS_FAILED'
+def start_UDP_server():
+    # socketserver is Python 3 only.  Don't import it in Python 2
+    import socketserver
 
-    def handle(self):
-        data = self.request[0].strip()
 
-        output = data.decode('utf-8')
-        print(output)
-        if output == self.quit_on:
-            sys.exit(1)
+    class MyUDPHandler(socketserver.BaseRequestHandler):
+
+        quit_on = 'TESTS_FAILED'
+
+        def handle(self):
+            data = self.request[0].strip()
+
+            output = data.decode('utf-8')
+            print(output)
+            if output == self.quit_on:
+                sys.exit(1)
 
 
-def start_UDP_server():
     HOST, PORT = "127.0.0.1", 9999
     with socketserver.UDPServer((HOST, PORT), MyUDPHandler) as server:
         server.serve_forever()
 
 def run_GH_file(gh_file, extra_env_vars):
+    
+    # multiprocessing is Python 3 only.  Don't import it in Python 2
+    import multiprocessing
+
+
     p = multiprocessing.Process(target=start_UDP_server)
     p.daemon = True
     print('Starting output printing UDP server.  Press Ctrl+C to quit.')
     p.start()
 
 
 
@@ -44,27 +52,27 @@
     # By default, exit Rhino afterwards.
     env['CHEETAH_GH_NON_INTERACTIVE'] = 'True'
 
 
     env.update(extra_env_vars)
 
 
-    print(rf'Opening: {gh_file}')
+    print('Opening: %s' % gh_file)
 
     command = ( 
-           r'"C:\Program Files\Rhino 8\System\Rhino.exe" /nosplash /runscript='
-          rf'"-_grasshopper _editor _load _document _open {gh_file} '
+          r'"C:\Program Files\Rhino 8\System\Rhino.exe" /nosplash /runscript='
+          r'"-_grasshopper _editor _load _document _open %s ' % gh_file
           )
 
     if env['CHEETAH_GH_NON_INTERACTIVE'].lower() not in ('', '0', 'false'):
         command += ' _enter _exit'
     command += ' _enterend"'
 
     result = subprocess.run(command, env=env, shell=True)
-    
+
     p.terminate()
 
     return result, p.exitcode
 
 
 
 
@@ -76,21 +84,21 @@
     # Subsequent trailing command line args are env variable names and values.
     other_args = iter(args[1:])
 
     extra_env_vars = dict(zip(other_args, other_args))
 
     result, exitcode = run_GH_file(gh_file = gh_file, extra_env_vars = extra_env_vars)
 
-    print(f'{result.returncode=}')
-    print(f'{exitcode=}')
+    print('result.returncode=%s' % result.returncode)
+    print('exitcode=%s' % exitcode)
 
     if result.returncode != 0 or exitcode: 
         raise Exception(
-             'An error occurred while running: {gh_file}. \n'
-            f'Test runner retcode: {result.returncode}\n'
-            f'Test output server exitcode: {exitcode}\n'
-            )
+             'An error occurred while running: %s. \n'
+             'Test runner retcode: %s\n'
+             'Test output server exitcode: %s\n'
+            ) % (gh_file, result.returncode, exitcode)
     return 0
 
 
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `cheetah_gh-0.1.4/src/Cheetah_GH/helpers.py` & `cheetah_gh-0.1.5/src/Cheetah_GH/helpers.py`

 * *Files identical despite different names*

### Comparing `cheetah_gh-0.1.4/src/Cheetah_GH/unittest_runner.py` & `cheetah_gh-0.1.5/src/Cheetah_GH/unittest_runner.py`

 * *Files identical despite different names*

### Comparing `cheetah_gh-0.1.4/.gitignore` & `cheetah_gh-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `cheetah_gh-0.1.4/pyproject.toml` & `cheetah_gh-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 
 
 
 [project]
 name = "Cheetah_GH"
-version = "0.1.4"
+version = "0.1.5"
 authors = [{name = "James Parrott", email = "james.parrott@proton.me"}]
 description = "Runs Grasshopper components and stops Rhino from Python components. Optionally runs Rhino3D and Grasshopper from the command line."
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=2.7"
 keywords = ["Rhino", "Grasshopper", "control", "components", "runner", "tests"]
 license = {file = "LICENSE.md"}
 classifiers = [
```

### Comparing `cheetah_gh-0.1.4/PKG-INFO` & `cheetah_gh-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.3
 Name: Cheetah_GH
-Version: 0.1.4
+Version: 0.1.5
 Summary: Runs Grasshopper components and stops Rhino from Python components. Optionally runs Rhino3D and Grasshopper from the command line.
 Project-URL: Homepage, https://github.com/JamesParrott/Cheetah_GH
 Project-URL: Bug Tracker, https://github.com/JamesParrott/Cheetah_GH/issues
 Author-email: James Parrott <james.parrott@proton.me>
 License-File: LICENSE.md
 Keywords: Grasshopper,Rhino,components,control,runner,tests
 Classifier: Programming Language :: Python
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
 
 # Cheetah
 Cheetah runs Grasshopper components, and runs Grasshopper from the command line.  Output from Python components in Grasshopper can be sent to the command line.  Cheetah can stop
-Grasshopper from a Python component, and return any exit code.
+Grasshopper from a Python component, and return any exit code.
+
+The CLI Rhino runner requires Python 3.
```

