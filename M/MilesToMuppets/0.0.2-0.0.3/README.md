# Comparing `tmp/milestomuppets-0.0.2.tar.gz` & `tmp/milestomuppets-0.0.3.tar.gz`

## Comparing `milestomuppets-0.0.2.tar` & `milestomuppets-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 milestomuppets-0.0.2/src/milesToMuppets/__init__.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 milestomuppets-0.0.2/src/milesToMuppets/data.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 milestomuppets-0.0.2/src/milesToMuppets/functions.py
--rw-r--r--   0        0        0     3851 2020-02-02 00:00:00.000000 milestomuppets-0.0.2/src/milesToMuppets/muppet.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 milestomuppets-0.0.2/src/milesToMuppets/txt/links.txt
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 milestomuppets-0.0.2/src/milesToMuppets/txt/notes.txt
--rw-r--r--   0        0        0     5776 2020-02-02 00:00:00.000000 milestomuppets-0.0.2/tests/legacy.py
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 milestomuppets-0.0.2/tests/tmp
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 milestomuppets-0.0.2/LICENSE
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 milestomuppets-0.0.2/README.md
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 milestomuppets-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 milestomuppets-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 milestomuppets-0.0.3/src/milesToMuppets/__init__.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 milestomuppets-0.0.3/src/milesToMuppets/data.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 milestomuppets-0.0.3/src/milesToMuppets/functions.py
+-rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 milestomuppets-0.0.3/src/milesToMuppets/muppet.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 milestomuppets-0.0.3/src/milesToMuppets/txt/links.txt
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 milestomuppets-0.0.3/src/milesToMuppets/txt/notes.txt
+-rw-r--r--   0        0        0     5776 2020-02-02 00:00:00.000000 milestomuppets-0.0.3/tests/legacy.py
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 milestomuppets-0.0.3/tests/tmp
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 milestomuppets-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 milestomuppets-0.0.3/README.md
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 milestomuppets-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 milestomuppets-0.0.3/PKG-INFO
```

### Comparing `milestomuppets-0.0.2/src/milesToMuppets/functions.py` & `milestomuppets-0.0.3/src/milesToMuppets/functions.py`

 * *Files identical despite different names*

### Comparing `milestomuppets-0.0.2/src/milesToMuppets/muppet.py` & `milestomuppets-0.0.3/src/milesToMuppets/muppet.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import sys
 import time
 
 # imports
 import requests
 
 # files
-from data import *
-from functions import *
+from .data import *
+from .functions import *
 
 class MilesToMuppets:
     def __init__(self, client_id: str, client_secret: str, output_mode: str= 'null') -> None:
         # set up internal 
         DATA = data
         CONSTANTS = DATA['constants']
         KEY_LIST = DATA['key_list']
```

### Comparing `milestomuppets-0.0.2/tests/legacy.py` & `milestomuppets-0.0.3/tests/legacy.py`

 * *Files identical despite different names*

### Comparing `milestomuppets-0.0.2/LICENSE` & `milestomuppets-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `milestomuppets-0.0.2/README.md` & `milestomuppets-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `milestomuppets-0.0.2/pyproject.toml` & `milestomuppets-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "src/milesToMuppets",
     "src/data",
     "src/functions"
 ]
 
 [project]
 name = "MilesToMuppets"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Sketched Doughnut", email="author@example.com" },
 ]
 description = "A conversion package to convert Miles to how many songs you can listen to from the Muppets Album"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `milestomuppets-0.0.2/PKG-INFO` & `milestomuppets-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: MilesToMuppets
-Version: 0.0.2
+Version: 0.0.3
 Summary: A conversion package to convert Miles to how many songs you can listen to from the Muppets Album
 Author-email: Sketched Doughnut <author@example.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
```

