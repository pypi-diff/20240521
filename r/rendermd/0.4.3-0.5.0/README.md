# Comparing `tmp/rendermd-0.4.3.tar.gz` & `tmp/rendermd-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rendermd-0.4.3.tar", last modified: Tue Dec  1 04:02:18 2020, max compression
+gzip compressed data, was "rendermd-0.5.0.tar", last modified: Tue May 21 18:13:38 2024, max compression
```

## Comparing `rendermd-0.4.3.tar` & `rendermd-0.5.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-01 04:02:18.089479 rendermd-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (116)      161 2020-12-01 04:01:50.000000 rendermd-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     1861 2020-12-01 04:02:18.089479 rendermd-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1102 2020-12-01 04:01:50.000000 rendermd-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (116)     1073 2020-12-01 04:01:50.000000 rendermd-0.4.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)       98 2020-12-01 04:01:50.000000 rendermd-0.4.3/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)      225 2020-12-01 04:01:50.000000 rendermd-0.4.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-01 04:02:18.089479 rendermd-0.4.3/rendermd/
--rw-r--r--   0 runner    (1001) docker     (116)       45 2020-12-01 04:01:50.000000 rendermd-0.4.3/rendermd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       13 2020-12-01 04:01:50.000000 rendermd-0.4.3/rendermd/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (116)     1169 2020-12-01 04:01:50.000000 rendermd-0.4.3/rendermd/command_line.py
--rw-r--r--   0 runner    (1001) docker     (116)      406 2020-12-01 04:01:50.000000 rendermd-0.4.3/rendermd/command_line.pyi
--rw-r--r--   0 runner    (1001) docker     (116)     1069 2020-12-01 04:01:50.000000 rendermd-0.4.3/rendermd/command_parser.py
--rw-r--r--   0 runner    (1001) docker     (116)      285 2020-12-01 04:01:50.000000 rendermd-0.4.3/rendermd/command_parser.pyi
--rw-r--r--   0 runner    (1001) docker     (116)      371 2020-12-01 04:01:50.000000 rendermd-0.4.3/rendermd/core.py
--rw-r--r--   0 runner    (1001) docker     (116)      288 2020-12-01 04:01:50.000000 rendermd-0.4.3/rendermd/core.pyi
--rw-r--r--   0 runner    (1001) docker     (116)      886 2020-12-01 04:01:50.000000 rendermd-0.4.3/rendermd/printer.py
--rw-r--r--   0 runner    (1001) docker     (116)      431 2020-12-01 04:01:50.000000 rendermd-0.4.3/rendermd/printer.pyi
--rw-r--r--   0 runner    (1001) docker     (116)     1908 2020-12-01 04:01:50.000000 rendermd-0.4.3/rendermd/shell.py
--rw-r--r--   0 runner    (1001) docker     (116)      329 2020-12-01 04:01:50.000000 rendermd-0.4.3/rendermd/shell.pyi
--rw-r--r--   0 runner    (1001) docker     (116)     1525 2020-12-01 04:01:50.000000 rendermd-0.4.3/rendermd/toc.py
--rw-r--r--   0 runner    (1001) docker     (116)      318 2020-12-01 04:01:50.000000 rendermd-0.4.3/rendermd/toc.pyi
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-01 04:02:18.089479 rendermd-0.4.3/rendermd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1861 2020-12-01 04:02:17.000000 rendermd-0.4.3/rendermd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      593 2020-12-01 04:02:17.000000 rendermd-0.4.3/rendermd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-01 04:02:17.000000 rendermd-0.4.3/rendermd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       57 2020-12-01 04:02:17.000000 rendermd-0.4.3/rendermd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       27 2020-12-01 04:02:17.000000 rendermd-0.4.3/rendermd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2020-12-01 04:02:17.000000 rendermd-0.4.3/rendermd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      189 2020-12-01 04:01:50.000000 rendermd-0.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)      826 2020-12-01 04:02:18.093479 rendermd-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1171 2020-12-01 04:01:50.000000 rendermd-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:13:38.447411 rendermd-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-21 18:13:18.000000 rendermd-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-21 18:13:18.000000 rendermd-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-21 18:13:38.447411 rendermd-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-21 18:13:18.000000 rendermd-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-21 18:13:18.000000 rendermd-0.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-21 18:13:18.000000 rendermd-0.5.0/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-21 18:13:18.000000 rendermd-0.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:13:38.447411 rendermd-0.5.0/rendermd/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-21 18:13:18.000000 rendermd-0.5.0/rendermd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 18:13:18.000000 rendermd-0.5.0/rendermd/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-21 18:13:18.000000 rendermd-0.5.0/rendermd/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-21 18:13:18.000000 rendermd-0.5.0/rendermd/command_line.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-21 18:13:18.000000 rendermd-0.5.0/rendermd/command_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-21 18:13:18.000000 rendermd-0.5.0/rendermd/command_parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-21 18:13:18.000000 rendermd-0.5.0/rendermd/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-21 18:13:18.000000 rendermd-0.5.0/rendermd/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-21 18:13:18.000000 rendermd-0.5.0/rendermd/printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-21 18:13:18.000000 rendermd-0.5.0/rendermd/printer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-21 18:13:18.000000 rendermd-0.5.0/rendermd/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-21 18:13:18.000000 rendermd-0.5.0/rendermd/shell.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-21 18:13:18.000000 rendermd-0.5.0/rendermd/toc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-21 18:13:18.000000 rendermd-0.5.0/rendermd/toc.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:13:38.447411 rendermd-0.5.0/rendermd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-21 18:13:38.000000 rendermd-0.5.0/rendermd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-21 18:13:38.000000 rendermd-0.5.0/rendermd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 18:13:38.000000 rendermd-0.5.0/rendermd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-21 18:13:38.000000 rendermd-0.5.0/rendermd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-21 18:13:38.000000 rendermd-0.5.0/rendermd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 18:13:38.000000 rendermd-0.5.0/rendermd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-21 18:13:18.000000 rendermd-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-21 18:13:38.447411 rendermd-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-21 18:13:18.000000 rendermd-0.5.0/setup.py
```

### Comparing `rendermd-0.4.3/PKG-INFO` & `rendermd-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 Metadata-Version: 2.1
 Name: rendermd
-Version: 0.4.3
+Version: 0.5.0
 Summary: Python type code generator
 Home-page: https://github.com/conanfanli/rendermd
 Author: Conan Li
 Author-email: conanlics@gmail.com
 License: MIT
 Description: 
         Table of Contents
         =================
         
         
         * `renderme <#renderme>`_
+        * `Installation <#installation>`_
         * `Usage <#usage>`_
         
           * `Examples: <#examples>`_
         
         renderme
         ========
         
-        Render markdown templates.
+        Render markdown templates by injecting table of contents and shell command output.
+        
+        Installation
+        ============
+        
+        ``pip install renderme``
         
         Usage
         =====
         
         .. code-block::
         
            usage: rendermd [-h] [-p PATTERNS] [--no-recursive]
@@ -47,9 +53,9 @@
         * More examples can be found in `test_toc_generator.py <./tests/test_toc_generator.py>`_ and `test_shell_generator.py <./tests/test_shell_generator.py>`_
         
 Keywords: Python,TypeScript,Dataclass,Code Generation
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: ~=3.8
+Requires-Python: ~=3.11
 Provides-Extra: dev
```

### Comparing `rendermd-0.4.3/README.md` & `rendermd-0.5.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 
 [//]: # (start:toc)
 Table of Contents
 =================
 - [renderme](#renderme)
+- [Installation](#installation)
 - [Usage](#usage)
     - [Examples:](#examples)
 
 [//]: # (end)
 
 # renderme
 
-Render markdown templates.
+Render markdown templates by injecting table of contents and shell command output.
+
+# Installation
+
+`pip install renderme`
 
 # Usage
 [//]: # (start:shell`python -m rendermd.command_line --help`)
 ```
 usage: rendermd [-h] [-p PATTERNS] [--no-recursive]
 
 Render markdown templates. This command recursively search the current
```

### Comparing `rendermd-0.4.3/README.rst` & `rendermd-0.5.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 
 Table of Contents
 =================
 
 
 * `renderme <#renderme>`_
+* `Installation <#installation>`_
 * `Usage <#usage>`_
 
   * `Examples: <#examples>`_
 
 renderme
 ========
 
-Render markdown templates.
+Render markdown templates by injecting table of contents and shell command output.
+
+Installation
+============
+
+``pip install renderme``
 
 Usage
 =====
 
 .. code-block::
 
    usage: rendermd [-h] [-p PATTERNS] [--no-recursive]
```

### Comparing `rendermd-0.4.3/rendermd/command_line.py` & `rendermd-0.5.0/rendermd/command_line.py`

 * *Files identical despite different names*

### Comparing `rendermd-0.4.3/rendermd/command_parser.py` & `rendermd-0.5.0/rendermd/command_parser.py`

 * *Files identical despite different names*

### Comparing `rendermd-0.4.3/rendermd/printer.py` & `rendermd-0.5.0/rendermd/printer.py`

 * *Files identical despite different names*

### Comparing `rendermd-0.4.3/rendermd/shell.py` & `rendermd-0.5.0/rendermd/shell.py`

 * *Files identical despite different names*

### Comparing `rendermd-0.4.3/rendermd/toc.py` & `rendermd-0.5.0/rendermd/toc.py`

 * *Files identical despite different names*

### Comparing `rendermd-0.4.3/rendermd.egg-info/PKG-INFO` & `rendermd-0.5.0/rendermd.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 Metadata-Version: 2.1
 Name: rendermd
-Version: 0.4.3
+Version: 0.5.0
 Summary: Python type code generator
 Home-page: https://github.com/conanfanli/rendermd
 Author: Conan Li
 Author-email: conanlics@gmail.com
 License: MIT
 Description: 
         Table of Contents
         =================
         
         
         * `renderme <#renderme>`_
+        * `Installation <#installation>`_
         * `Usage <#usage>`_
         
           * `Examples: <#examples>`_
         
         renderme
         ========
         
-        Render markdown templates.
+        Render markdown templates by injecting table of contents and shell command output.
+        
+        Installation
+        ============
+        
+        ``pip install renderme``
         
         Usage
         =====
         
         .. code-block::
         
            usage: rendermd [-h] [-p PATTERNS] [--no-recursive]
@@ -47,9 +53,9 @@
         * More examples can be found in `test_toc_generator.py <./tests/test_toc_generator.py>`_ and `test_shell_generator.py <./tests/test_shell_generator.py>`_
         
 Keywords: Python,TypeScript,Dataclass,Code Generation
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: ~=3.8
+Requires-Python: ~=3.11
 Provides-Extra: dev
```

### Comparing `rendermd-0.4.3/rendermd.egg-info/SOURCES.txt` & `rendermd-0.5.0/rendermd.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 README.rst
 dev-requirements.txt
 pyproject.toml
 requirements.txt
 setup.cfg
```

### Comparing `rendermd-0.4.3/setup.cfg` & `rendermd-0.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `rendermd-0.4.3/setup.py` & `rendermd-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     name="rendermd",
     version=VERSION,
     description="Python type code generator",
     long_description=long_description,
     url="https://github.com/conanfanli/rendermd",
     packages=find_packages(exclude=["tests"]),
     include_package_data=True,
-    python_requires="~=3.8",
+    python_requires="~=3.11",
     install_requires=[
         "md-toc",
     ],
     extras_require={"dev": ["ipython", "mypy"]},
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: MIT License",
```

