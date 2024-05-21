# Comparing `tmp/fa-essentials-1.0.98.tar.gz` & `tmp/fa-essentials-1.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fa-essentials-1.0.98.tar", last modified: Mon Jan  8 15:12:03 2024, max compression
+gzip compressed data, was "fa-essentials-1.0.99.tar", last modified: Mon Jan  8 15:20:25 2024, max compression
```

## Comparing `fa-essentials-1.0.98.tar` & `fa-essentials-1.0.99.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 15:12:03.106529 fa-essentials-1.0.98/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-01-08 15:11:40.000000 fa-essentials-1.0.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-01-08 15:12:03.102529 fa-essentials-1.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-01-08 15:11:40.000000 fa-essentials-1.0.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 15:12:03.102529 fa-essentials-1.0.98/fa_essentials.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-01-08 15:12:03.000000 fa-essentials-1.0.98/fa_essentials.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-01-08 15:12:03.000000 fa-essentials-1.0.98/fa_essentials.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-08 15:12:03.000000 fa-essentials-1.0.98/fa_essentials.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-01-08 15:12:03.000000 fa-essentials-1.0.98/fa_essentials.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-08 15:12:03.000000 fa-essentials-1.0.98/fa_essentials.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 15:12:03.102529 fa-essentials-1.0.98/faessentials/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 15:11:40.000000 fa-essentials-1.0.98/faessentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-01-08 15:11:40.000000 fa-essentials-1.0.98/faessentials/asset_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-01-08 15:11:40.000000 fa-essentials-1.0.98/faessentials/global_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-01-08 15:11:40.000000 fa-essentials-1.0.98/faessentials/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-01-08 15:11:40.000000 fa-essentials-1.0.98/faessentials/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-01-08 15:11:56.000000 fa-essentials-1.0.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-08 15:12:03.106529 fa-essentials-1.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-01-08 15:11:40.000000 fa-essentials-1.0.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 15:12:03.102529 fa-essentials-1.0.98/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-01-08 15:11:40.000000 fa-essentials-1.0.98/tests/test_asset_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-01-08 15:11:40.000000 fa-essentials-1.0.98/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 15:20:25.702635 fa-essentials-1.0.99/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-01-08 15:20:05.000000 fa-essentials-1.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-01-08 15:20:25.702635 fa-essentials-1.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-01-08 15:20:05.000000 fa-essentials-1.0.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 15:20:25.702635 fa-essentials-1.0.99/fa_essentials.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-01-08 15:20:25.000000 fa-essentials-1.0.99/fa_essentials.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-01-08 15:20:25.000000 fa-essentials-1.0.99/fa_essentials.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-08 15:20:25.000000 fa-essentials-1.0.99/fa_essentials.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-01-08 15:20:25.000000 fa-essentials-1.0.99/fa_essentials.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-08 15:20:25.000000 fa-essentials-1.0.99/fa_essentials.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 15:20:25.698635 fa-essentials-1.0.99/faessentials/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 15:20:05.000000 fa-essentials-1.0.99/faessentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-01-08 15:20:05.000000 fa-essentials-1.0.99/faessentials/asset_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-01-08 15:20:05.000000 fa-essentials-1.0.99/faessentials/global_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-01-08 15:20:05.000000 fa-essentials-1.0.99/faessentials/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-01-08 15:20:05.000000 fa-essentials-1.0.99/faessentials/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-01-08 15:20:18.000000 fa-essentials-1.0.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-08 15:20:25.702635 fa-essentials-1.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-01-08 15:20:05.000000 fa-essentials-1.0.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 15:20:25.702635 fa-essentials-1.0.99/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-01-08 15:20:05.000000 fa-essentials-1.0.99/tests/test_asset_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-01-08 15:20:05.000000 fa-essentials-1.0.99/tests/test_utils.py
```

### Comparing `fa-essentials-1.0.98/LICENSE` & `fa-essentials-1.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `fa-essentials-1.0.98/PKG-INFO` & `fa-essentials-1.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-essentials
-Version: 1.0.98
+Version: 1.0.99
 Summary: Essentials for our projects.
 Author-email: Brayan <brayan@sparkandhale.com>
 Project-URL: Homepage, https://github.com/svabra/fa-essentials
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
```

### Comparing `fa-essentials-1.0.98/README.md` & `fa-essentials-1.0.99/README.md`

 * *Files identical despite different names*

### Comparing `fa-essentials-1.0.98/fa_essentials.egg-info/PKG-INFO` & `fa-essentials-1.0.99/fa_essentials.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-essentials
-Version: 1.0.98
+Version: 1.0.99
 Summary: Essentials for our projects.
 Author-email: Brayan <brayan@sparkandhale.com>
 Project-URL: Homepage, https://github.com/svabra/fa-essentials
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
```

### Comparing `fa-essentials-1.0.98/faessentials/asset_formatter.py` & `fa-essentials-1.0.99/faessentials/asset_formatter.py`

 * *Files identical despite different names*

### Comparing `fa-essentials-1.0.98/faessentials/global_logger.py` & `fa-essentials-1.0.99/faessentials/global_logger.py`

 * *Files identical despite different names*

### Comparing `fa-essentials-1.0.98/faessentials/utils.py` & `fa-essentials-1.0.99/faessentials/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 PROJECT_ROOT = None
 
 def find_project_root(current_path: pathlib.Path, max_depth: int = 10) -> pathlib.Path:
     """
     Recursively search for a marker (like the 'config' or 'logs' directory) to find the project root.
     """
     for _ in range(max_depth):
-        if (current_path / "config").exists() or (current_path / "logs").exists():            
+        if (current_path / "config").exists() or (current_path / "logs").exists():
             return current_path
         current_path = current_path.parent
     raise FileNotFoundError(f"Could not find the project root. Ensure the 'config' or 'logs' folder exists in {current_path.name}")
 
 # Initialize PROJECT_ROOT when the module is loaded
 def initialize_project_root():
     global PROJECT_ROOT
-    PROJECT_ROOT = find_project_root(pathlib.Path(__file__).resolve())    
+    PROJECT_ROOT = find_project_root(pathlib.Path(__file__).resolve())
 
 initialize_project_root()
 
 def get_project_root_path() -> Path:
     """
     Return the project root path.
     """
```

### Comparing `fa-essentials-1.0.98/pyproject.toml` & `fa-essentials-1.0.99/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=66.1.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fa-essentials"
-version = "1.0.98"
+version = "1.0.99"
 description = "Essentials for our projects."
 readme = "README.md"
 authors = [{ name = "Brayan", email = "brayan@sparkandhale.com" }]
 #license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python"
@@ -25,15 +25,15 @@
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/svabra/fa-essentials"
 
 [tool.bumpver]
-current_version = "1.0.98"
+current_version = "1.0.99"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fa-essentials-1.0.98/setup.py` & `fa-essentials-1.0.99/setup.py`

 * *Files identical despite different names*

### Comparing `fa-essentials-1.0.98/tests/test_asset_formatter.py` & `fa-essentials-1.0.99/tests/test_asset_formatter.py`

 * *Files identical despite different names*

### Comparing `fa-essentials-1.0.98/tests/test_utils.py` & `fa-essentials-1.0.99/tests/test_utils.py`

 * *Files identical despite different names*

