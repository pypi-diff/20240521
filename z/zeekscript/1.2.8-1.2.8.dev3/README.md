# Comparing `tmp/zeekscript-1.2.8.tar.gz` & `tmp/zeekscript-1.2.8.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeekscript-1.2.8.tar", last modified: Fri Dec  1 10:29:38 2023, max compression
+gzip compressed data, was "zeekscript-1.2.8.dev3.tar", last modified: Tue May 21 09:27:58 2024, max compression
```

## Comparing `zeekscript-1.2.8.tar` & `zeekscript-1.2.8.dev3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 10:29:38.815868 zeekscript-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2023-12-01 10:29:35.000000 zeekscript-1.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      259 2023-12-01 10:29:35.000000 zeekscript-1.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8814 2023-12-01 10:29:38.815868 zeekscript-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8271 2023-12-01 10:29:35.000000 zeekscript-1.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-01 10:29:35.000000 zeekscript-1.2.8/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       92 2023-12-01 10:29:35.000000 zeekscript-1.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-01 10:29:38.815868 zeekscript-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2023-12-01 10:29:35.000000 zeekscript-1.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 10:29:38.807869 zeekscript-1.2.8/tree-sitter-zeek/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 10:29:38.807869 zeekscript-1.2.8/tree-sitter-zeek/src/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2023-12-01 10:29:37.000000 zeekscript-1.2.8/tree-sitter-zeek/src/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      321 2023-12-01 10:29:37.000000 zeekscript-1.2.8/tree-sitter-zeek/src/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    96658 2023-12-01 10:29:37.000000 zeekscript-1.2.8/tree-sitter-zeek/src/grammar.json
--rw-r--r--   0 runner    (1001) docker     (127)    24299 2023-12-01 10:29:37.000000 zeekscript-1.2.8/tree-sitter-zeek/src/node-types.json
--rw-r--r--   0 runner    (1001) docker     (127)  4495479 2023-12-01 10:29:37.000000 zeekscript-1.2.8/tree-sitter-zeek/src/parser.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 10:29:38.811869 zeekscript-1.2.8/tree-sitter-zeek/src/tree_sitter/
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2023-12-01 10:29:37.000000 zeekscript-1.2.8/tree-sitter-zeek/src/tree_sitter/parser.h
--rwxr-xr-x   0 runner    (1001) docker     (127)     1253 2023-12-01 10:29:35.000000 zeekscript-1.2.8/zeek-format
--rwxr-xr-x   0 runner    (1001) docker     (127)     2041 2023-12-01 10:29:35.000000 zeekscript-1.2.8/zeek-script
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 10:29:38.815868 zeekscript-1.2.8/zeekscript/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2023-12-01 10:29:35.000000 zeekscript-1.2.8/zeekscript/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6407 2023-12-01 10:29:35.000000 zeekscript-1.2.8/zeekscript/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2023-12-01 10:29:35.000000 zeekscript-1.2.8/zeekscript/error.py
--rw-r--r--   0 runner    (1001) docker     (127)    52769 2023-12-01 10:29:35.000000 zeekscript-1.2.8/zeekscript/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11727 2023-12-01 10:29:35.000000 zeekscript-1.2.8/zeekscript/node.py
--rw-r--r--   0 runner    (1001) docker     (127)    11963 2023-12-01 10:29:35.000000 zeekscript-1.2.8/zeekscript/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2023-12-01 10:29:35.000000 zeekscript-1.2.8/zeekscript/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    19447 2023-12-01 10:29:35.000000 zeekscript-1.2.8/zeekscript/script.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 10:29:38.815868 zeekscript-1.2.8/zeekscript.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8814 2023-12-01 10:29:38.000000 zeekscript-1.2.8/zeekscript.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      625 2023-12-01 10:29:38.000000 zeekscript-1.2.8/zeekscript.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-01 10:29:38.000000 zeekscript-1.2.8/zeekscript.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-01 10:29:38.000000 zeekscript-1.2.8/zeekscript.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-01 10:29:38.000000 zeekscript-1.2.8/zeekscript.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:27:58.221029 zeekscript-1.2.8.dev3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-21 09:27:53.000000 zeekscript-1.2.8.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-21 09:27:53.000000 zeekscript-1.2.8.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8819 2024-05-21 09:27:58.221029 zeekscript-1.2.8.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8271 2024-05-21 09:27:53.000000 zeekscript-1.2.8.dev3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-21 09:27:53.000000 zeekscript-1.2.8.dev3/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-21 09:27:53.000000 zeekscript-1.2.8.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 09:27:58.221029 zeekscript-1.2.8.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-21 09:27:53.000000 zeekscript-1.2.8.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:27:58.209029 zeekscript-1.2.8.dev3/tree-sitter-zeek/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:27:58.213029 zeekscript-1.2.8.dev3/tree-sitter-zeek/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-21 09:27:56.000000 zeekscript-1.2.8.dev3/tree-sitter-zeek/src/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-21 09:27:56.000000 zeekscript-1.2.8.dev3/tree-sitter-zeek/src/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    96658 2024-05-21 09:27:56.000000 zeekscript-1.2.8.dev3/tree-sitter-zeek/src/grammar.json
+-rw-r--r--   0 runner    (1001) docker     (127)    24299 2024-05-21 09:27:56.000000 zeekscript-1.2.8.dev3/tree-sitter-zeek/src/node-types.json
+-rw-r--r--   0 runner    (1001) docker     (127)  4495479 2024-05-21 09:27:56.000000 zeekscript-1.2.8.dev3/tree-sitter-zeek/src/parser.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:27:58.217029 zeekscript-1.2.8.dev3/tree-sitter-zeek/src/tree_sitter/
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-05-21 09:27:56.000000 zeekscript-1.2.8.dev3/tree-sitter-zeek/src/tree_sitter/parser.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1253 2024-05-21 09:27:53.000000 zeekscript-1.2.8.dev3/zeek-format
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2041 2024-05-21 09:27:53.000000 zeekscript-1.2.8.dev3/zeek-script
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:27:58.217029 zeekscript-1.2.8.dev3/zeekscript/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-21 09:27:53.000000 zeekscript-1.2.8.dev3/zeekscript/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-05-21 09:27:53.000000 zeekscript-1.2.8.dev3/zeekscript/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-21 09:27:53.000000 zeekscript-1.2.8.dev3/zeekscript/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52769 2024-05-21 09:27:53.000000 zeekscript-1.2.8.dev3/zeekscript/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11727 2024-05-21 09:27:53.000000 zeekscript-1.2.8.dev3/zeekscript/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11963 2024-05-21 09:27:53.000000 zeekscript-1.2.8.dev3/zeekscript/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-21 09:27:53.000000 zeekscript-1.2.8.dev3/zeekscript/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19447 2024-05-21 09:27:53.000000 zeekscript-1.2.8.dev3/zeekscript/script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:27:58.221029 zeekscript-1.2.8.dev3/zeekscript.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8819 2024-05-21 09:27:58.000000 zeekscript-1.2.8.dev3/zeekscript.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-21 09:27:58.000000 zeekscript-1.2.8.dev3/zeekscript.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:27:58.000000 zeekscript-1.2.8.dev3/zeekscript.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-21 09:27:58.000000 zeekscript-1.2.8.dev3/zeekscript.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-21 09:27:58.000000 zeekscript-1.2.8.dev3/zeekscript.egg-info/top_level.txt
```

### Comparing `zeekscript-1.2.8/LICENSE` & `zeekscript-1.2.8.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `zeekscript-1.2.8/PKG-INFO` & `zeekscript-1.2.8.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: zeekscript
-Version: 1.2.8
+Version: 1.2.8.dev3
 Summary: A Zeek script formatter and analyzer
 Home-page: https://github.com/zeek/zeekscript
 Maintainer: The Zeek Project
 Maintainer-email: info@zeek.org
 License: UNKNOWN
 Keywords: zeek scripts language formatter formatting indenter indenting parsing
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Utilities
-Requires-Python: >3.7.0
+Requires-Python: >3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # A toolchain to parse, analyze, and format Zeek scripts
 
 [![Build and test](https://github.com/zeek/zeekscript/actions/workflows/build_wheels.yml/badge.svg)](https://github.com/zeek/zeekscript/actions/workflows/build_wheels.yml)
```

### Comparing `zeekscript-1.2.8/README.md` & `zeekscript-1.2.8.dev3/README.md`

 * *Files identical despite different names*

### Comparing `zeekscript-1.2.8/setup.py` & `zeekscript-1.2.8.dev3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,16 +75,16 @@
     packages=["zeekscript"],
     package_data={"zeekscript": ["zeek-language.so"]},
     cmdclass={
         "build_py": BuildCommand,
         "install": InstallPlatlib,
     },
     distclass=BinaryDistribution,
-    setup_requires=["tree_sitter"],
-    install_requires=["tree_sitter"],
-    python_requires=">3.7.0",
+    setup_requires=["tree_sitter==0.21.3"],
+    install_requires=["tree_sitter==0.21.3"],
+    python_requires=">3.8.0",
     classifiers=[
         "Programming Language :: Python :: 3.7",
         "License :: OSI Approved :: BSD License",
         "Topic :: Utilities",
     ],
 )
```

### Comparing `zeekscript-1.2.8/tree-sitter-zeek/src/grammar.json` & `zeekscript-1.2.8.dev3/tree-sitter-zeek/src/grammar.json`

 * *Files identical despite different names*

### Comparing `zeekscript-1.2.8/tree-sitter-zeek/src/node-types.json` & `zeekscript-1.2.8.dev3/tree-sitter-zeek/src/node-types.json`

 * *Files identical despite different names*

### Comparing `zeekscript-1.2.8/tree-sitter-zeek/src/parser.c` & `zeekscript-1.2.8.dev3/tree-sitter-zeek/src/parser.c`

 * *Files identical despite different names*

### Comparing `zeekscript-1.2.8/tree-sitter-zeek/src/tree_sitter/parser.h` & `zeekscript-1.2.8.dev3/tree-sitter-zeek/src/tree_sitter/parser.h`

 * *Files identical despite different names*

### Comparing `zeekscript-1.2.8/zeek-format` & `zeekscript-1.2.8.dev3/zeek-format`

 * *Files identical despite different names*

### Comparing `zeekscript-1.2.8/zeek-script` & `zeekscript-1.2.8.dev3/zeek-script`

 * *Files identical despite different names*

### Comparing `zeekscript-1.2.8/zeekscript/cli.py` & `zeekscript-1.2.8.dev3/zeekscript/cli.py`

 * *Files identical despite different names*

### Comparing `zeekscript-1.2.8/zeekscript/formatter.py` & `zeekscript-1.2.8.dev3/zeekscript/formatter.py`

 * *Files identical despite different names*

### Comparing `zeekscript-1.2.8/zeekscript/node.py` & `zeekscript-1.2.8.dev3/zeekscript/node.py`

 * *Files identical despite different names*

### Comparing `zeekscript-1.2.8/zeekscript/output.py` & `zeekscript-1.2.8.dev3/zeekscript/output.py`

 * *Files identical despite different names*

### Comparing `zeekscript-1.2.8/zeekscript/parser.py` & `zeekscript-1.2.8.dev3/zeekscript/parser.py`

 * *Files identical despite different names*

### Comparing `zeekscript-1.2.8/zeekscript/script.py` & `zeekscript-1.2.8.dev3/zeekscript/script.py`

 * *Files identical despite different names*

### Comparing `zeekscript-1.2.8/zeekscript.egg-info/PKG-INFO` & `zeekscript-1.2.8.dev3/zeekscript.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: zeekscript
-Version: 1.2.8
+Version: 1.2.8.dev3
 Summary: A Zeek script formatter and analyzer
 Home-page: https://github.com/zeek/zeekscript
 Maintainer: The Zeek Project
 Maintainer-email: info@zeek.org
 License: UNKNOWN
 Keywords: zeek scripts language formatter formatting indenter indenting parsing
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Utilities
-Requires-Python: >3.7.0
+Requires-Python: >3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # A toolchain to parse, analyze, and format Zeek scripts
 
 [![Build and test](https://github.com/zeek/zeekscript/actions/workflows/build_wheels.yml/badge.svg)](https://github.com/zeek/zeekscript/actions/workflows/build_wheels.yml)
```

### Comparing `zeekscript-1.2.8/zeekscript.egg-info/SOURCES.txt` & `zeekscript-1.2.8.dev3/zeekscript.egg-info/SOURCES.txt`

 * *Files identical despite different names*

