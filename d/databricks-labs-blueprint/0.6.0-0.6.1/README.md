# Comparing `tmp/databricks_labs_blueprint-0.6.0.tar.gz` & `tmp/databricks_labs_blueprint-0.6.1.tar.gz`

## Comparing `databricks_labs_blueprint-0.6.0.tar` & `databricks_labs_blueprint-0.6.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/databricks/__init__.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/databricks/labs/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/__init__.py
--rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/__main__.py
--rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/cli.py
--rw-r--r--   0        0        0     8420 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/commands.py
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/entrypoint.py
--rw-r--r--   0        0        0    42934 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/installation.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/installer.py
--rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/limiter.py
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/logger.py
--rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/parallel.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/py.typed
--rw-r--r--   0        0        0     5590 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/tui.py
--rw-r--r--   0        0        0     6176 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/upgrades.py
--rw-r--r--   0        0        0    14208 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/wheels.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/.gitignore
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/LICENSE
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/NOTICE
--rw-r--r--   0        0        0    45992 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/README.md
--rw-r--r--   0        0        0    26290 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    46795 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/databricks/__init__.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/databricks/labs/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/__init__.py
+-rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/__main__.py
+-rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/cli.py
+-rw-r--r--   0        0        0     8420 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/commands.py
+-rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/entrypoint.py
+-rw-r--r--   0        0        0    42934 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/installation.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/installer.py
+-rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/limiter.py
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/logger.py
+-rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/parallel.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/py.typed
+-rw-r--r--   0        0        0     5590 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/tui.py
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/upgrades.py
+-rw-r--r--   0        0        0    14116 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/wheels.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/.gitignore
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/LICENSE
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/NOTICE
+-rw-r--r--   0        0        0    45992 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/README.md
+-rw-r--r--   0        0        0    26290 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0    46795 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.1/PKG-INFO
```

### Comparing `databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/__main__.py` & `databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/__main__.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/cli.py` & `databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/cli.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/commands.py` & `databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/commands.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/entrypoint.py` & `databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/entrypoint.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/installation.py` & `databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/installation.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/installer.py` & `databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/installer.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/limiter.py` & `databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/limiter.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/logger.py` & `databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/logger.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/parallel.py` & `databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/parallel.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/tui.py` & `databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/tui.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/upgrades.py` & `databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/upgrades.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     def apply(self, ws: WorkspaceClient):
         """Applies application state upgrades for the given installation."""
         upgrades_folder = self._product_info.version_file().parent / "upgrades"
         if not upgrades_folder.exists():
             logger.warning(f"No upgrades folder: {upgrades_folder}")
             return
         applied = self._installation.load_or_default(AppliedUpgrades)
-        for script in self._diff(upgrades_folder):
+        for script in sorted(self._diff(upgrades_folder)):
             if script.name in applied.upgrades:
                 logger.info(f"Already applied: {script.name}")
                 continue
             self._apply_python_script(script, ws)
             applied.upgrades.append(script.name)
             self._installation.save(applied)
```

### Comparing `databricks_labs_blueprint-0.6.0/databricks/labs/blueprint/wheels.py` & `databricks_labs_blueprint-0.6.1/databricks/labs/blueprint/wheels.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,24 +70,24 @@
 
         The path to this package can be thought as a way to determine the other
         assets of your deployed wheel.
 
         See https://packaging.python.org/guides/single-sourcing-package-version/"""
         return self._version_file
 
-    def version(self):
+    @cached_property
+    def _version(self):
         """Returns current version of the project"""
-        if hasattr(self, "__version"):
-            return self.__version  # pylint: disable=access-member-before-definition
         if not self.is_git_checkout():
             # normal install, downloaded releases won't have the .git folder
-            self.__version = self.released_version()
-            return self.__version
-        self.__version = self.unreleased_version()
-        return self.__version
+            return self.released_version()
+        return self.unreleased_version()
+
+    def version(self):
+        return self._version
 
     def as_semver(self) -> SemVer:
         """Returns the version as SemVer object."""
         return SemVer.parse(self.version())
 
     def product_name(self) -> str:
         """Returns the product name based on the version file folder name."""
@@ -330,12 +330,17 @@
         return tmp_dir_path
 
 
 class Wheels(WheelsV2):
     """Wheel builder"""
 
     def __init__(
-        self, ws: WorkspaceClient, install_state: InstallState, product_info: ProductInfo, *, verbose: bool = False
+        self,
+        ws: WorkspaceClient,
+        install_state: InstallState,
+        product_info: ProductInfo,
+        *,
+        verbose: bool = False,
     ):
         warnings.warn("Wheels is deprecated, use WheelsV2 instead", DeprecationWarning)
         installation = Installation(ws, product_info.product_name(), install_folder=install_state.install_folder())
         super().__init__(installation, product_info, verbose=verbose)
```

### Comparing `databricks_labs_blueprint-0.6.0/.gitignore` & `databricks_labs_blueprint-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.0/LICENSE` & `databricks_labs_blueprint-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.0/README.md` & `databricks_labs_blueprint-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.0/pyproject.toml` & `databricks_labs_blueprint-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.0/PKG-INFO` & `databricks_labs_blueprint-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: databricks-labs-blueprint
-Version: 0.6.0
+Version: 0.6.1
 Summary: Common libraries for Databricks Labs
 Project-URL: Issues, https://github.com/databrickslabs/blueprint/issues
 Project-URL: Source, https://github.com/databrickslabs/blueprint
 License-File: LICENSE
 License-File: NOTICE
 Keywords: Databricks
 Classifier: Development Status :: 3 - Alpha
```

