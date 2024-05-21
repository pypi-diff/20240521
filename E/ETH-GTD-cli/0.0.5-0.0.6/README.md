# Comparing `tmp/eth_gtd_cli-0.0.5.tar.gz` & `tmp/eth_gtd_cli-0.0.6.tar.gz`

## Comparing `eth_gtd_cli-0.0.5.tar` & `eth_gtd_cli-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.5/.idea/.gitignore
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.5/.idea/CLI.iml
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.5/.idea/misc.xml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.5/.idea/modules.xml
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.5/.idea/vcs.xml
--rw-r--r--   0        0        0     8397 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.5/.idea/workspace.xml
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.5/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.5/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.5/src/ETH_GTD_cli/__init__.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.5/src/ETH_GTD_cli/consts.py
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.5/src/ETH_GTD_cli/helper.py
--rw-r--r--   0        0        0     6247 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.5/src/ETH_GTD_cli/main.py
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.5/LICENSE
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.5/README.md
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.6/.idea/.gitignore
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.6/.idea/CLI.iml
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.6/.idea/misc.xml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.6/.idea/modules.xml
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.6/.idea/vcs.xml
+-rw-r--r--   0        0        0     8397 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.6/.idea/workspace.xml
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.6/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.6/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.6/src/ETH_GTD_cli/__init__.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.6/src/ETH_GTD_cli/consts.py
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.6/src/ETH_GTD_cli/helper.py
+-rw-r--r--   0        0        0     6247 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.6/src/ETH_GTD_cli/main.py
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.6/LICENSE
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.6/README.md
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.6/PKG-INFO
```

### Comparing `eth_gtd_cli-0.0.5/.idea/workspace.xml` & `eth_gtd_cli-0.0.6/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.5/.idea/inspectionProfiles/Project_Default.xml` & `eth_gtd_cli-0.0.6/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.5/src/ETH_GTD_cli/helper.py` & `eth_gtd_cli-0.0.6/src/ETH_GTD_cli/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import threading
 
 import httpx
 import tqdm
 from rich import print
 import queue
 
-from consts import API_URL
+from .consts import API_URL
 
 
 def list_files_recursive(path, recursive: bool, pattern: str, depth: int = 0):
     files = []
     res = {}
     try:
         entries = os.listdir(path)
```

### Comparing `eth_gtd_cli-0.0.5/src/ETH_GTD_cli/main.py` & `eth_gtd_cli-0.0.6/src/ETH_GTD_cli/main.py`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.5/LICENSE` & `eth_gtd_cli-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.5/pyproject.toml` & `eth_gtd_cli-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ETH_GTD_cli"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Johann Schwabe", email="jschwab@ethz.ch" },
 ]
 description = "A CLI for the ETH project Grand Tour"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
```

### Comparing `eth_gtd_cli-0.0.5/PKG-INFO` & `eth_gtd_cli-0.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ETH_GTD_cli
-Version: 0.0.5
+Version: 0.0.6
 Summary: A CLI for the ETH project Grand Tour
 Project-URL: Homepage, https://github.com/leggedrobotics/GrandTourDatasets
 Project-URL: Issues, https://github.com/leggedrobotics/GrandTourDatasets/issues
 Author-email: Johann Schwabe <jschwab@ethz.ch>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

