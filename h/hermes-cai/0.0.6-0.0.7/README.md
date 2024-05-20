# Comparing `tmp/hermes_cai-0.0.6.tar.gz` & `tmp/hermes_cai-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hermes_cai-0.0.6.tar", last modified: Mon May 20 21:56:33 2024, max compression
+gzip compressed data, was "hermes_cai-0.0.7.tar", last modified: Mon May 20 22:20:36 2024, max compression
```

## Comparing `hermes_cai-0.0.6.tar` & `hermes_cai-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 21:56:33.182781 hermes_cai-0.0.6/
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)       15 2024-05-20 21:56:28.000000 hermes_cai-0.0.6/MANIFEST.in
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)     3563 2024-05-20 21:56:33.182597 hermes_cai-0.0.6/PKG-INFO
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)     3220 2024-05-20 20:22:55.000000 hermes_cai-0.0.6/README.md
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)        5 2024-05-20 21:56:32.000000 hermes_cai-0.0.6/VERSION
-drwxr-xr-x   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 21:56:33.181168 hermes_cai-0.0.6/hermes_cai/
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 20:22:55.000000 hermes_cai-0.0.6/hermes_cai/__init__.py
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)      556 2024-05-20 20:54:56.000000 hermes_cai-0.0.6/hermes_cai/constants.py
-drwxr-xr-x   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 21:56:33.182284 hermes_cai-0.0.6/hermes_cai.egg-info/
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)     3563 2024-05-20 21:56:33.000000 hermes_cai-0.0.6/hermes_cai.egg-info/PKG-INFO
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)      221 2024-05-20 21:56:33.000000 hermes_cai-0.0.6/hermes_cai.egg-info/SOURCES.txt
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)        1 2024-05-20 21:56:33.000000 hermes_cai-0.0.6/hermes_cai.egg-info/dependency_links.txt
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)       11 2024-05-20 21:56:33.000000 hermes_cai-0.0.6/hermes_cai.egg-info/top_level.txt
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)       38 2024-05-20 21:56:33.182995 hermes_cai-0.0.6/setup.cfg
--rw-r--r--   0 jamesgroeneveld   (501) staff       (20)      867 2024-05-20 21:54:39.000000 hermes_cai-0.0.6/setup.py
+drwxr-xr-x   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 22:20:36.894822 hermes_cai-0.0.7/
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)       16 2024-05-20 22:15:52.000000 hermes_cai-0.0.7/MANIFEST.in
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)     3563 2024-05-20 22:20:36.894644 hermes_cai-0.0.7/PKG-INFO
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)     3220 2024-05-20 22:15:52.000000 hermes_cai-0.0.7/README.md
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)        5 2024-05-20 22:20:35.000000 hermes_cai-0.0.7/VERSION
+drwxr-xr-x   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 22:20:36.893829 hermes_cai-0.0.7/hermes_cai/
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 22:15:52.000000 hermes_cai-0.0.7/hermes_cai/__init__.py
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)      556 2024-05-20 22:15:52.000000 hermes_cai-0.0.7/hermes_cai/constants.py
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)      625 2024-05-20 20:17:08.000000 hermes_cai-0.0.7/hermes_cai/exceptions.py
+drwxr-xr-x   0 jamesgroeneveld   (501) staff       (20)        0 2024-05-20 22:20:36.894461 hermes_cai-0.0.7/hermes_cai.egg-info/
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)     3563 2024-05-20 22:20:36.000000 hermes_cai-0.0.7/hermes_cai.egg-info/PKG-INFO
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)      246 2024-05-20 22:20:36.000000 hermes_cai-0.0.7/hermes_cai.egg-info/SOURCES.txt
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)        1 2024-05-20 22:20:36.000000 hermes_cai-0.0.7/hermes_cai.egg-info/dependency_links.txt
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)       11 2024-05-20 22:20:36.000000 hermes_cai-0.0.7/hermes_cai.egg-info/top_level.txt
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)       38 2024-05-20 22:20:36.894854 hermes_cai-0.0.7/setup.cfg
+-rw-r--r--   0 jamesgroeneveld   (501) staff       (20)      868 2024-05-20 22:15:52.000000 hermes_cai-0.0.7/setup.py
```

### Comparing `hermes_cai-0.0.6/PKG-INFO` & `hermes_cai-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hermes-cai
-Version: 0.0.6
+Version: 0.0.7
 Summary: Defining and constructing production-grade prompts via an expressive templating engine.
 Home-page: https://github.com/character-tech/chat-stack
 Author: James Groeneveld
 Author-email: james@character.ai
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `hermes_cai-0.0.6/README.md` & `hermes_cai-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `hermes_cai-0.0.6/hermes_cai/constants.py` & `hermes_cai-0.0.7/hermes_cai/constants.py`

 * *Files identical despite different names*

### Comparing `hermes_cai-0.0.6/hermes_cai.egg-info/PKG-INFO` & `hermes_cai-0.0.7/hermes_cai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hermes-cai
-Version: 0.0.6
+Version: 0.0.7
 Summary: Defining and constructing production-grade prompts via an expressive templating engine.
 Home-page: https://github.com/character-tech/chat-stack
 Author: James Groeneveld
 Author-email: james@character.ai
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `hermes_cai-0.0.6/setup.py` & `hermes_cai-0.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Setup file for the Hermes package."""
 
-from setuptools import find_packages, setup
 import os
 
+from setuptools import find_packages, setup
+
 # Get the current directory of the setup.py script
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Read the version from the VERSION file
-with open(os.path.join(here, 'VERSION')) as version_file:
+with open(os.path.join(here, "VERSION")) as version_file:
     version = version_file.read().strip()
 
 setup(
     name="hermes-cai",
     version=version,
     packages=find_packages(include=["hermes_cai", "hermes_cai.*"]),
     install_requires=[],
```

