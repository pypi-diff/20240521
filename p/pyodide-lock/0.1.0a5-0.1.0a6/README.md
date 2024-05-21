# Comparing `tmp/pyodide_lock-0.1.0a5.tar.gz` & `tmp/pyodide_lock-0.1.0a6.tar.gz`

## Comparing `pyodide_lock-0.1.0a5.tar` & `pyodide_lock-0.1.0a6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/.codecov.yml
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/CHANGELOG.md
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/.github/workflows/main.yml
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/pyodide_lock/__init__.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/pyodide_lock/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/pyodide_lock/py.typed
--rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/pyodide_lock/spec.py
--rw-r--r--   0        0        0    13898 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/pyodide_lock/utils.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/tests/conftest.py
--rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/tests/test_spec.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/tests/test_utils.py
--rw-r--r--   0        0        0     7193 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/tests/test_wheel.py
--rw-r--r--   0        0        0    14988 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/tests/data/pyodide-lock-0.22.1.json.gz
--rw-r--r--   0        0        0    16292 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/tests/data/pyodide-lock-0.23.3.json.gz
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/.gitignore
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/LICENSE
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/README.md
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/pyproject.toml
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a5/PKG-INFO
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a6/.codecov.yml
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a6/CHANGELOG.md
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a6/.github/workflows/main.yml
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a6/pyodide_lock/__init__.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a6/pyodide_lock/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a6/pyodide_lock/py.typed
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a6/pyodide_lock/spec.py
+-rw-r--r--   0        0        0    13930 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a6/pyodide_lock/utils.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a6/tests/conftest.py
+-rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a6/tests/test_spec.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a6/tests/test_utils.py
+-rw-r--r--   0        0        0     7193 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a6/tests/test_wheel.py
+-rw-r--r--   0        0        0    14988 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a6/tests/data/pyodide-lock-0.22.1.json.gz
+-rw-r--r--   0        0        0    16292 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a6/tests/data/pyodide-lock-0.23.3.json.gz
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a6/.gitignore
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a6/LICENSE
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a6/README.md
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a6/pyproject.toml
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 pyodide_lock-0.1.0a6/PKG-INFO
```

### Comparing `pyodide_lock-0.1.0a5/.pre-commit-config.yaml` & `pyodide_lock-0.1.0a6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyodide_lock-0.1.0a5/CHANGELOG.md` & `pyodide_lock-0.1.0a6/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,21 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## Unreleased
 
+## [0.1.0a6] - 2024-04-03
+
+### Added
+
+- The `info` field now contains an optional `abi_version`.
+  [#86](https://github.com/pyodide/pyodide-lock/pull/86)
+
 ## [0.1.0a5] - 2024-04-03
 
 ### Changed
 
 - `pydantic >= 2.0` is now required.
   [#26](https://github.com/pyodide/pyodide-lock/pull/26)
```

### Comparing `pyodide_lock-0.1.0a5/.github/workflows/main.yml` & `pyodide_lock-0.1.0a6/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pyodide_lock-0.1.0a5/pyodide_lock/cli.py` & `pyodide_lock-0.1.0a6/pyodide_lock/cli.py`

 * *Files identical despite different names*

### Comparing `pyodide_lock-0.1.0a5/pyodide_lock/spec.py` & `pyodide_lock-0.1.0a6/pyodide_lock/spec.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 
 class InfoSpec(BaseModel):
     arch: Literal["wasm32", "wasm64"] = "wasm32"
     platform: str
     version: str
     python: str
+    abi_version: str | None = None
     model_config = ConfigDict(extra="forbid")
 
 
 class PackageSpec(BaseModel):
     name: str
     version: str
     file_name: str = Field(
```

### Comparing `pyodide_lock-0.1.0a5/pyodide_lock/utils.py` & `pyodide_lock-0.1.0a6/pyodide_lock/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     with open(full_path, "rb") as f:
         while chunk := f.read(4096):
             sha256_hash.update(chunk)
     return sha256_hash.hexdigest()
 
 
 def _get_marker_environment(
-    platform: str, version: str, arch: str, python: str
+    platform: str, version: str, arch: str, python: str, abi_version: str | None = None
 ) -> dict[str, str]:
     """
     Get the marker environment for this pyodide-lock file. If running
     inside pyodide it returns the current marker environment.
     """
     if "pyodide" in sys.modules:
         from packaging.markers import default_environment
```

### Comparing `pyodide_lock-0.1.0a5/tests/conftest.py` & `pyodide_lock-0.1.0a6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyodide_lock-0.1.0a5/tests/test_spec.py` & `pyodide_lock-0.1.0a6/tests/test_spec.py`

 * *Files identical despite different names*

### Comparing `pyodide_lock-0.1.0a5/tests/test_utils.py` & `pyodide_lock-0.1.0a6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyodide_lock-0.1.0a5/tests/test_wheel.py` & `pyodide_lock-0.1.0a6/tests/test_wheel.py`

 * *Files identical despite different names*

### Comparing `pyodide_lock-0.1.0a5/tests/data/pyodide-lock-0.22.1.json.gz` & `pyodide_lock-0.1.0a6/tests/data/pyodide-lock-0.22.1.json.gz`

 * *Files identical despite different names*

### Comparing `pyodide_lock-0.1.0a5/tests/data/pyodide-lock-0.23.3.json.gz` & `pyodide_lock-0.1.0a6/tests/data/pyodide-lock-0.23.3.json.gz`

 * *Files identical despite different names*

### Comparing `pyodide_lock-0.1.0a5/LICENSE` & `pyodide_lock-0.1.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodide_lock-0.1.0a5/README.md` & `pyodide_lock-0.1.0a6/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_lock-0.1.0a5/pyproject.toml` & `pyodide_lock-0.1.0a6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyodide_lock-0.1.0a5/PKG-INFO` & `pyodide_lock-0.1.0a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyodide-lock
-Version: 0.1.0a5
+Version: 0.1.0a6
 Summary: Tooling to manage the `pyodide-lock.json` file
 Project-URL: Homepage, https://github.com/pyodide/pyodide-lock
 Project-URL: Bug Tracker, https://github.com/pyodide/pyodide-lock/issues
 Author: Pyodide developers
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

