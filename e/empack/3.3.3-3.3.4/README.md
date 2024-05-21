# Comparing `tmp/empack-3.3.3.tar.gz` & `tmp/empack-3.3.4.tar.gz`

## Comparing `empack-3.3.3.tar` & `empack-3.3.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 empack-3.3.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3775 2020-02-02 00:00:00.000000 empack-3.3.3/CHANGELOG.md
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 empack-3.3.3/ci_env.yml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 empack-3.3.3/setup.py
--rw-r--r--   0        0        0     5109 2020-02-02 00:00:00.000000 empack-3.3.3/config/empack_config.yaml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 empack-3.3.3/empack/__init__.py
--rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 empack-3.3.3/empack/file_patterns.py
--rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 empack-3.3.3/empack/filter_env.py
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 empack-3.3.3/empack/micromamba_wrapper.py
--rw-r--r--   0        0        0    10233 2020-02-02 00:00:00.000000 empack-3.3.3/empack/pack.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 empack-3.3.3/empack/repodata.py
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 empack-3.3.3/empack/tar_utils.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 empack-3.3.3/empack/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 empack-3.3.3/empack/cli/__init__.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 empack-3.3.3/empack/cli/app.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 empack-3.3.3/empack/cli/err.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 empack-3.3.3/empack/cli/main.py
--rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 empack-3.3.3/empack/cli/pack.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 empack-3.3.3/empack/cli/repodata.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 empack-3.3.3/empack/cli/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 empack-3.3.3/tests/__init__.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 empack-3.3.3/tests/conftest.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 empack-3.3.3/tests/empack_test_config.yaml
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 empack-3.3.3/tests/empack_test_extra_config.yaml
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 empack-3.3.3/tests/test_cli.py
--rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 empack-3.3.3/tests/test_filter.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 empack-3.3.3/tests/test_integration.py
--rw-r--r--   0        0        0     7872 2020-02-02 00:00:00.000000 empack-3.3.3/tests/test_pack.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 empack-3.3.3/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 empack-3.3.3/LICENSE
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 empack-3.3.3/README.md
--rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 empack-3.3.3/pyproject.toml
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 empack-3.3.3/PKG-INFO
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 empack-3.3.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 empack-3.3.4/CHANGELOG.md
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 empack-3.3.4/ci_env.yml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 empack-3.3.4/setup.py
+-rw-r--r--   0        0        0     5313 2020-02-02 00:00:00.000000 empack-3.3.4/config/empack_config.yaml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 empack-3.3.4/empack/__init__.py
+-rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 empack-3.3.4/empack/file_patterns.py
+-rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 empack-3.3.4/empack/filter_env.py
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 empack-3.3.4/empack/micromamba_wrapper.py
+-rw-r--r--   0        0        0    10233 2020-02-02 00:00:00.000000 empack-3.3.4/empack/pack.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 empack-3.3.4/empack/repodata.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 empack-3.3.4/empack/tar_utils.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 empack-3.3.4/empack/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 empack-3.3.4/empack/cli/__init__.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 empack-3.3.4/empack/cli/app.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 empack-3.3.4/empack/cli/err.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 empack-3.3.4/empack/cli/main.py
+-rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 empack-3.3.4/empack/cli/pack.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 empack-3.3.4/empack/cli/repodata.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 empack-3.3.4/empack/cli/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 empack-3.3.4/tests/__init__.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 empack-3.3.4/tests/conftest.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 empack-3.3.4/tests/empack_test_config.yaml
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 empack-3.3.4/tests/empack_test_extra_config.yaml
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 empack-3.3.4/tests/test_cli.py
+-rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 empack-3.3.4/tests/test_filter.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 empack-3.3.4/tests/test_integration.py
+-rw-r--r--   0        0        0     7872 2020-02-02 00:00:00.000000 empack-3.3.4/tests/test_pack.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 empack-3.3.4/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 empack-3.3.4/LICENSE
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 empack-3.3.4/README.md
+-rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 empack-3.3.4/pyproject.toml
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 empack-3.3.4/PKG-INFO
```

### Comparing `empack-3.3.3/.pre-commit-config.yaml` & `empack-3.3.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `empack-3.3.3/CHANGELOG.md` & `empack-3.3.4/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,27 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 3.3.4
+
+([Full Changelog](https://github.com/emscripten-forge/empack/compare/v3.3.3...784118763a5fd903569df7b1ef686a9c54eaa1e4))
+
+### Enhancements made
+
+- Add Include/Exclude Patterns for `pint` Package to `empack_config` (#2) [#97](https://github.com/emscripten-forge/empack/pull/97) ([@michaelweinold](https://github.com/michaelweinold))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/emscripten-forge/empack/graphs/contributors?from=2024-04-26&to=2024-05-21&type=c))
+
+[@martinRenou](https://github.com/search?q=repo%3Aemscripten-forge%2Fempack+involves%3AmartinRenou+updated%3A2024-04-26..2024-05-21&type=Issues) | [@michaelweinold](https://github.com/search?q=repo%3Aemscripten-forge%2Fempack+involves%3Amichaelweinold+updated%3A2024-04-26..2024-05-21&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 3.3.3
 
 ([Full Changelog](https://github.com/emscripten-forge/empack/compare/v3.3.2...d6ae4fc42fe79aa7a60f4b70fa72245e1e7566a3))
 
 ### Enhancements made
 
 - use abspath when comparing dirs [#95](https://github.com/emscripten-forge/empack/pull/95) ([@DerThorsten](https://github.com/DerThorsten))
@@ -17,16 +33,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/emscripten-forge/empack/graphs/contributors?from=2024-02-05&to=2024-04-26&type=c))
 
 [@DerThorsten](https://github.com/search?q=repo%3Aemscripten-forge%2Fempack+involves%3ADerThorsten+updated%3A2024-02-05..2024-04-26&type=Issues) | [@martinRenou](https://github.com/search?q=repo%3Aemscripten-forge%2Fempack+involves%3AmartinRenou+updated%3A2024-02-05..2024-04-26&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 3.3.2
 
 ([Full Changelog](https://github.com/emscripten-forge/empack/compare/v3.3.1...d742539ef5f7fdf4afb94561d4026a7976ebc629))
 
 ### Enhancements made
 
 - Update config for urllib and certifi [#94](https://github.com/emscripten-forge/empack/pull/94) ([@martinRenou](https://github.com/martinRenou))
```

### Comparing `empack-3.3.3/config/empack_config.yaml` & `empack-3.3.4/config/empack_config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -153,14 +153,22 @@
     include_patterns:
       - pattern: '*.py'
       - pattern: '*.pem'
   pyvis:
     include_patterns:
       - pattern: '*.py'
       - pattern: '*.html'
+  pint:
+     include_patterns:
+       - pattern: '*.so'
+       - pattern: '*.py'
+       - pattern: '*.txt'
+     exclude_patterns:
+       - pattern: '**/tests/**/*.py'
+       - pattern: '**/tests/**/*.so'
 default:
   include_patterns:
     - pattern: '*.so'
     - pattern: '*.py'
     - pattern: '*.json'
     - pattern: 'share/zoneinfo/**'
     - pattern: '**/*.dist-info/METADATA'
```

### Comparing `empack-3.3.3/empack/file_patterns.py` & `empack-3.3.4/empack/file_patterns.py`

 * *Files identical despite different names*

### Comparing `empack-3.3.3/empack/filter_env.py` & `empack-3.3.4/empack/filter_env.py`

 * *Files identical despite different names*

### Comparing `empack-3.3.3/empack/micromamba_wrapper.py` & `empack-3.3.4/empack/micromamba_wrapper.py`

 * *Files identical despite different names*

### Comparing `empack-3.3.3/empack/pack.py` & `empack-3.3.4/empack/pack.py`

 * *Files identical despite different names*

### Comparing `empack-3.3.3/empack/repodata.py` & `empack-3.3.4/empack/repodata.py`

 * *Files identical despite different names*

### Comparing `empack-3.3.3/empack/tar_utils.py` & `empack-3.3.4/empack/tar_utils.py`

 * *Files identical despite different names*

### Comparing `empack-3.3.3/empack/cli/pack.py` & `empack-3.3.4/empack/cli/pack.py`

 * *Files identical despite different names*

### Comparing `empack-3.3.3/empack/cli/repodata.py` & `empack-3.3.4/empack/cli/repodata.py`

 * *Files identical despite different names*

### Comparing `empack-3.3.3/tests/conftest.py` & `empack-3.3.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `empack-3.3.3/tests/empack_test_config.yaml` & `empack-3.3.4/tests/empack_test_config.yaml`

 * *Files identical despite different names*

### Comparing `empack-3.3.3/tests/test_cli.py` & `empack-3.3.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `empack-3.3.3/tests/test_filter.py` & `empack-3.3.4/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `empack-3.3.3/tests/test_integration.py` & `empack-3.3.4/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `empack-3.3.3/tests/test_pack.py` & `empack-3.3.4/tests/test_pack.py`

 * *Files identical despite different names*

### Comparing `empack-3.3.3/.gitignore` & `empack-3.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `empack-3.3.3/LICENSE` & `empack-3.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `empack-3.3.3/README.md` & `empack-3.3.4/README.md`

 * *Files identical despite different names*

### Comparing `empack-3.3.3/pyproject.toml` & `empack-3.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `empack-3.3.3/PKG-INFO` & `empack-3.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: empack
-Version: 3.3.3
+Version: 3.3.4
 Summary: empack emscripten+boa
 Project-URL: Homepage, https://github.com/emscripten-forge/empack
 Author-email: Thorsten Beier <derthorstenbeier@gmail.com>
 License: 
         MIT License
         
         Copyright (c) 2022, Thorsten Beier
```

