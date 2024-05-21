# Comparing `tmp/validate_pyproject_schema_store-2024.5.13.tar.gz` & `tmp/validate_pyproject_schema_store-2024.5.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon May 13 23:51:26 2024, max compression
+gzip compressed data, last modified: Tue May 21 04:55:19 2024, max compression
```

## Comparing `validate_pyproject_schema_store-2024.5.13.tar` & `validate_pyproject_schema_store-2024.5.20.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     2273 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/.pre-commit-config.yaml
--rw-r--r--   0        0        0      305 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0     2412 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/.github/release.yml
--rw-r--r--   0        0        0      668 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/.github/matchers/pylint.json
--rw-r--r--   0        0        0     1093 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/.github/workflows/bump.yml
--rw-r--r--   0        0        0      843 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/.github/workflows/cd.yml
--rw-r--r--   0        0        0      885 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/.github/workflows/ci.yml
--rw-r--r--   0        0        0      188 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/py.typed
--rw-r--r--   0        0        0     1373 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/schema.py
--rw-r--r--   0        0        0     6871 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/black.schema.json
--rw-r--r--   0        0        0    20516 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/cibuildwheel.schema.json
--rw-r--r--   0        0        0    27093 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/hatch.schema.json
--rw-r--r--   0        0        0    44330 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/mypy.schema.json
--rw-r--r--   0        0        0    25354 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/pdm.schema.json
--rw-r--r--   0        0        0    20027 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/poetry.schema.json
--rw-r--r--   0        0        0    70996 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/pyright.schema.json
--rw-r--r--   0        0        0   128445 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/ruff.schema.json
--rw-r--r--   0        0        0    20535 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/scikit-build.schema.json
--rw-r--r--   0        0        0    13647 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/setuptools.schema.json
--rw-r--r--   0        0        0      691 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/tool.json
--rw-r--r--   0        0        0    24630 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/uv.schema.json
--rw-r--r--   0        0        0      890 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/tests/test_package.py
--rw-r--r--   0        0        0      850 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/tests/test_validate_pyproject.py
--rwxr-xr-x   0        0        0     2467 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/tools/sync.py
--rw-r--r--   0        0        0     2218 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/.gitignore
--rw-r--r--   0        0        0    11358 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/LICENSE
--rw-r--r--   0        0        0     2080 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/README.md
--rw-r--r--   0        0        0     4986 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/pyproject.toml
--rw-r--r--   0        0        0     4156 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/PKG-INFO
+-rw-r--r--   0        0        0     2273 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      305 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0     2412 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/.github/release.yml
+-rw-r--r--   0        0        0      668 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     1093 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/.github/workflows/bump.yml
+-rw-r--r--   0        0        0      843 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/.github/workflows/cd.yml
+-rw-r--r--   0        0        0      885 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      188 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/py.typed
+-rw-r--r--   0        0        0     1373 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/schema.py
+-rw-r--r--   0        0        0     6871 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/black.schema.json
+-rw-r--r--   0        0        0    20516 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/cibuildwheel.schema.json
+-rw-r--r--   0        0        0    27093 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/hatch.schema.json
+-rw-r--r--   0        0        0    44330 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/mypy.schema.json
+-rw-r--r--   0        0        0    25354 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/pdm.schema.json
+-rw-r--r--   0        0        0    20027 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/poetry.schema.json
+-rw-r--r--   0        0        0    70835 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/pyright.schema.json
+-rw-r--r--   0        0        0   128445 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/ruff.schema.json
+-rw-r--r--   0        0        0    20535 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/scikit-build.schema.json
+-rw-r--r--   0        0        0    13647 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/setuptools.schema.json
+-rw-r--r--   0        0        0      691 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/tool.json
+-rw-r--r--   0        0        0    24630 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/uv.schema.json
+-rw-r--r--   0        0        0      890 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/tests/test_package.py
+-rw-r--r--   0        0        0      850 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/tests/test_validate_pyproject.py
+-rwxr-xr-x   0        0        0     2467 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/tools/sync.py
+-rw-r--r--   0        0        0     2218 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/.gitignore
+-rw-r--r--   0        0        0    11358 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/LICENSE
+-rw-r--r--   0        0        0     2080 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/README.md
+-rw-r--r--   0        0        0     4986 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/pyproject.toml
+-rw-r--r--   0        0        0     4156 2024-05-21 04:55:19.000000 validate_pyproject_schema_store-2024.5.20/PKG-INFO
```

### Comparing `validate_pyproject_schema_store-2024.5.13/.pre-commit-config.yaml` & `validate_pyproject_schema_store-2024.5.20/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
       - id: disallow-caps
         name: Disallow improper capitalization
         language: pygrep
         entry: PyBind|Numpy|Cmake|CCache|Github|PyTest
         exclude: .pre-commit-config.yaml
 
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.17
+    rev: v0.18
     hooks:
       - id: validate-pyproject
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
     rev: 0.28.3
     hooks:
       - id: check-dependabot
```

### Comparing `validate_pyproject_schema_store-2024.5.13/.github/CONTRIBUTING.md` & `validate_pyproject_schema_store-2024.5.20/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.13/.github/matchers/pylint.json` & `validate_pyproject_schema_store-2024.5.20/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.13/.github/workflows/bump.yml` & `validate_pyproject_schema_store-2024.5.20/.github/workflows/bump.yml`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.13/.github/workflows/cd.yml` & `validate_pyproject_schema_store-2024.5.20/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.13/.github/workflows/ci.yml` & `validate_pyproject_schema_store-2024.5.20/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/schema.py` & `validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/schema.py`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/black.schema.json` & `validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/black.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/cibuildwheel.schema.json` & `validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/cibuildwheel.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/hatch.schema.json` & `validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/hatch.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/mypy.schema.json` & `validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/mypy.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/pdm.schema.json` & `validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/pdm.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/poetry.schema.json` & `validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/poetry.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/pyright.schema.json` & `validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/pyright.schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998764600179694%*

 * *Differences: {"'properties'": "{'strict': {'description': 'Paths of directories or files that should use "*

 * *                 '"strict" analysis if they are included. This is the same as manually adding a `# '*

 * *                 'pyright: strict` comment. In strict mode, most type-checking rules are enabled. '*

 * *                 'Paths may contain wildcard characters: `**` (a directory or multiple levels of '*

 * *                 'directories), `*` (a sequence of zero or more characters), or `?` (a single '*

 * *                 "char […]*

```diff
@@ -395,15 +395,15 @@
             "default": "error",
             "description": "Generate or suppress diagnostics for invalid type argument usage.",
             "title": "Controls reporting of invalid type argument usage"
         },
         "reportInvalidTypeForm": {
             "$id": "#/properties/reportInvalidTypeForm",
             "$ref": "#/definitions/diagnostic",
-            "default": "warning",
+            "default": "error",
             "description": "Generate or suppress diagnostics for type annotations that use invalid type expression forms or are semantically invalid.",
             "title": "Controls reporting of type expressions that use an invalid form"
         },
         "reportInvalidTypeVarUse": {
             "$id": "#/properties/reportInvalidTypeVarUse",
             "$ref": "#/definitions/diagnostic",
             "default": "warning",
@@ -455,15 +455,15 @@
             "default": "none",
             "description": "Generate or suppress diagnostics when a generic class is used without providing explicit or implicit type arguments.",
             "title": "Controls reporting generic class reference with missing type arguments"
         },
         "reportMissingTypeStubs": {
             "$id": "#/properties/reportMissingTypeStubs",
             "$ref": "#/definitions/diagnostic",
-            "default": "warning",
+            "default": "none",
             "description": "Generate or suppress diagnostics for imports that have no corresponding type stub file (either a typeshed file or a custom type stub). The type checker requires type stubs to do its best job at analysis.",
             "title": "Controls reporting of imports that cannot be resolved to type stub files"
         },
         "reportNoOverloadImplementation": {
             "$id": "#/properties/reportNoOverloadImplementation",
             "$ref": "#/definitions/diagnostic",
             "default": "error",
@@ -812,24 +812,24 @@
             "$ref": "#/definitions/diagnostic",
             "default": "warning",
             "description": "Generate or suppress diagnostics for a wildcard import from an external library. The use of this language feature is highly discouraged and can result in bugs when the library is updated.",
             "title": "Controls reporting of wildcard import from external library"
         },
         "strict": {
             "$id": "#/properties/strict",
-            "description": "Paths of directories or files that should use \"strict\" analysis if they are included. This is the same as manually adding a `# pyright: strict` comment. In strict mode, most type-checking rules are enabled. Refer to this table for details about which rules are enabled in strict mode. Paths may contain wildcard characters: `**` (a directory or multiple levels of directories), `*` (a sequence of zero or more characters), or `?` (a single character).",
+            "description": "Paths of directories or files that should use \"strict\" analysis if they are included. This is the same as manually adding a `# pyright: strict` comment. In strict mode, most type-checking rules are enabled. Paths may contain wildcard characters: `**` (a directory or multiple levels of directories), `*` (a sequence of zero or more characters), or `?` (a single character).",
             "items": {
                 "$id": "#/properties/strict/items",
                 "pattern": "^(.*)$",
                 "title": "File or directory that should use \"strict\" type checking rules",
                 "type": "string"
             },
             "title": "Files and directories that should use \"strict\" type checking rules",
             "type": "array",
-            "x-intellij-html-description": "Paths of directories or files that should use &quot;strict&quot; analysis if they are included. This is the same as manually adding a <code># pyright: strict</code> comment. In strict mode, most type-checking rules are enabled. Refer to this table for details about which rules are enabled in strict mode. Paths may contain wildcard characters: <code>**</code> (a directory or multiple levels of directories), <code>*</code> (a sequence of zero or more characters), or <code>?</code> (a single character)."
+            "x-intellij-html-description": "Paths of directories or files that should use &quot;strict&quot; analysis if they are included. This is the same as manually adding a <code># pyright: strict</code> comment. In strict mode, most type-checking rules are enabled. Paths may contain wildcard characters: <code>**</code> (a directory or multiple levels of directories), <code>*</code> (a sequence of zero or more characters), or <code>?</code> (a single character)."
         },
         "strictDictionaryInference": {
             "$id": "#/properties/strictDictionaryInference",
             "default": false,
             "description": "When inferring the type of a dictionary's keys and values, use strict type assumptions. For example, the expression `{'a': 1, 'b': 'a'}` could be inferred to be of type `dict[str, Any]` or `dict[str, int | str]`. If this setting is `true`, it will use the latter (stricter) type.",
             "title": "Infer strict types for dictionary expressions",
             "type": "boolean",
```

### Comparing `validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/ruff.schema.json` & `validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/ruff.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/scikit-build.schema.json` & `validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/scikit-build.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/setuptools.schema.json` & `validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/setuptools.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/tool.json` & `validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/tool.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/uv.schema.json` & `validate_pyproject_schema_store-2024.5.20/src/validate_pyproject_schema_store/resources/uv.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.13/tests/test_package.py` & `validate_pyproject_schema_store-2024.5.20/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.13/tests/test_validate_pyproject.py` & `validate_pyproject_schema_store-2024.5.20/tests/test_validate_pyproject.py`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.13/tools/sync.py` & `validate_pyproject_schema_store-2024.5.20/tools/sync.py`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.13/.gitignore` & `validate_pyproject_schema_store-2024.5.20/.gitignore`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.13/LICENSE` & `validate_pyproject_schema_store-2024.5.20/LICENSE`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.13/README.md` & `validate_pyproject_schema_store-2024.5.20/README.md`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.5.13/pyproject.toml` & `validate_pyproject_schema_store-2024.5.20/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "validate-pyproject-schema-store"
-version = "2024.05.13"
+version = "2024.05.20"
 authors = [
   { name = "Henry Schreiner", email = "henryfs@princeton.edu" },
 ]
 description = "A plugin set for validate-pyproject and schema-store."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `validate_pyproject_schema_store-2024.5.13/PKG-INFO` & `validate_pyproject_schema_store-2024.5.20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: validate-pyproject-schema-store
-Version: 2024.5.13
+Version: 2024.5.20
 Summary: A plugin set for validate-pyproject and schema-store.
 Project-URL: Homepage, https://github.com/henryiii/validate-pyproject-schema-store
 Project-URL: Bug Tracker, https://github.com/henryiii/validate-pyproject-schema-store/issues
 Project-URL: Discussions, https://github.com/henryiii/validate-pyproject-schema-store/discussions
 Project-URL: Changelog, https://github.com/henryiii/validate-pyproject-schema-store/releases
 Author-email: Henry Schreiner <henryfs@princeton.edu>
 License-File: LICENSE
```

