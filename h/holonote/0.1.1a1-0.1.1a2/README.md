# Comparing `tmp/holonote-0.1.1a1.tar.gz` & `tmp/holonote-0.1.1a2.tar.gz`

## Comparing `holonote-0.1.1a1.tar` & `holonote-0.1.1a2.tar`

### file list

```diff
@@ -1,61 +1,67 @@
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 holonote-0.1.1a1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 holonote-0.1.1a1/.github/workflows/build.yaml
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 holonote-0.1.1a1/.github/workflows/docs.yaml
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 holonote-0.1.1a1/.github/workflows/jupyterlite.yaml
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 holonote-0.1.1a1/.github/workflows/test.yaml
--rw-r--r--   0        0        0     4226 2020-02-02 00:00:00.000000 holonote-0.1.1a1/doc/conf.py
--rw-r--r--   0        0        0    11085 2020-02-02 00:00:00.000000 holonote-0.1.1a1/doc/generate_modules.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 holonote-0.1.1a1/doc/index.md
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 holonote-0.1.1a1/doc/no_header_tutorial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 holonote-0.1.1a1/doc/_static/assets/.empty
--rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 holonote-0.1.1a1/doc/_static/assets/jupyterlite.svg
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 holonote-0.1.1a1/doc/_static/css/custom.css
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 holonote-0.1.1a1/doc/_templates/jupyterlitelink.html
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 holonote-0.1.1a1/doc/basics/index.md
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 holonote-0.1.1a1/doc/reference_manual/index.md
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 holonote-0.1.1a1/doc/tutorial/index.md
--rw-r--r--   0        0        0   498993 2020-02-02 00:00:00.000000 holonote-0.1.1a1/examples/assets/example.parquet
--rw-r--r--   0        0        0    16480 2020-02-02 00:00:00.000000 holonote-0.1.1a1/examples/basics/Basics.ipynb
--rw-r--r--   0        0        0    16488 2020-02-02 00:00:00.000000 holonote-0.1.1a1/examples/basics/Basics_2D.ipynb
--rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 holonote-0.1.1a1/examples/basics/MultiPlot.ipynb
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 holonote-0.1.1a1/examples/tutorial/00_Overview.ipynb
--rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 holonote-0.1.1a1/examples/tutorial/01_First_Annotation.ipynb
--rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 holonote-0.1.1a1/examples/tutorial/02_Multiple_Annotations.ipynb
--rw-r--r--   0        0        0     8860 2020-02-02 00:00:00.000000 holonote-0.1.1a1/examples/tutorial/03_Styling_of_Annotations.ipynb
--rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 holonote-0.1.1a1/examples/tutorial/04_Make_an_App.ipynb
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 holonote-0.1.1a1/examples/tutorial/05_Watch_Events.ipynb
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 holonote-0.1.1a1/holonote/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 holonote-0.1.1a1/holonote/_version.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 holonote-0.1.1a1/holonote/_warnings.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 holonote-0.1.1a1/holonote/annotate/__init__.py
--rw-r--r--   0        0        0    15638 2020-02-02 00:00:00.000000 holonote-0.1.1a1/holonote/annotate/annotator.py
--rw-r--r--   0        0        0    18854 2020-02-02 00:00:00.000000 holonote-0.1.1a1/holonote/annotate/connector.py
--rw-r--r--   0        0        0    19020 2020-02-02 00:00:00.000000 holonote-0.1.1a1/holonote/annotate/display.py
--rw-r--r--   0        0        0    13288 2020-02-02 00:00:00.000000 holonote-0.1.1a1/holonote/annotate/table.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 holonote-0.1.1a1/holonote/annotate/typing.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 holonote-0.1.1a1/holonote/app/__init__.py
--rw-r--r--   0        0        0     6982 2020-02-02 00:00:00.000000 holonote-0.1.1a1/holonote/app/panel.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 holonote-0.1.1a1/holonote/editor/__init__.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 holonote-0.1.1a1/holonote/editor/editors.py
--rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 holonote-0.1.1a1/holonote/tests/conftest.py
--rw-r--r--   0        0        0     7762 2020-02-02 00:00:00.000000 holonote-0.1.1a1/holonote/tests/test_annotation_table.py
--rw-r--r--   0        0        0    13275 2020-02-02 00:00:00.000000 holonote-0.1.1a1/holonote/tests/test_annotators_advanced.py
--rw-r--r--   0        0        0    17224 2020-02-02 00:00:00.000000 holonote-0.1.1a1/holonote/tests/test_annotators_basic.py
--rw-r--r--   0        0        0     6046 2020-02-02 00:00:00.000000 holonote-0.1.1a1/holonote/tests/test_annotators_element.py
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 holonote-0.1.1a1/holonote/tests/test_annotators_interface.py
--rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 holonote-0.1.1a1/holonote/tests/test_annotators_style.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 holonote-0.1.1a1/holonote/tests/test_app.py
--rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 holonote-0.1.1a1/holonote/tests/test_connectors.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 holonote-0.1.1a1/holonote/tests/util.py
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 holonote-0.1.1a1/holonote/tests/benchmark/test_benchmarks.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 holonote-0.1.1a1/scripts/example_testing.py
--rwxr-xr-x   0        0        0      191 2020-02-02 00:00:00.000000 holonote-0.1.1a1/scripts/conda/build.sh
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 holonote-0.1.1a1/scripts/conda/recipe/meta.yaml
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 holonote-0.1.1a1/scripts/jupyterlite/build.sh
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 holonote-0.1.1a1/scripts/jupyterlite/patch_lock.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 holonote-0.1.1a1/scripts/jupyterlite/update_lock.js
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 holonote-0.1.1a1/.gitignore
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 holonote-0.1.1a1/LICENSE.txt
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 holonote-0.1.1a1/README.md
--rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 holonote-0.1.1a1/pyproject.toml
--rw-r--r--   0        0        0     5949 2020-02-02 00:00:00.000000 holonote-0.1.1a1/PKG-INFO
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 holonote-0.1.1a2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 holonote-0.1.1a2/.github/workflows/build.yaml
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 holonote-0.1.1a2/.github/workflows/docs.yaml
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 holonote-0.1.1a2/.github/workflows/jupyterlite.yaml
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 holonote-0.1.1a2/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     4226 2020-02-02 00:00:00.000000 holonote-0.1.1a2/doc/conf.py
+-rw-r--r--   0        0        0    11085 2020-02-02 00:00:00.000000 holonote-0.1.1a2/doc/generate_modules.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 holonote-0.1.1a2/doc/index.md
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 holonote-0.1.1a2/doc/no_header_tutorial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 holonote-0.1.1a2/doc/_static/assets/.empty
+-rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 holonote-0.1.1a2/doc/_static/assets/jupyterlite.svg
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 holonote-0.1.1a2/doc/_static/css/custom.css
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 holonote-0.1.1a2/doc/_templates/jupyterlitelink.html
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 holonote-0.1.1a2/doc/basics/index.md
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 holonote-0.1.1a2/doc/reference_manual/index.md
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 holonote-0.1.1a2/doc/tutorial/index.md
+-rw-r--r--   0        0        0   498993 2020-02-02 00:00:00.000000 holonote-0.1.1a2/examples/assets/example.parquet
+-rw-r--r--   0        0        0    16480 2020-02-02 00:00:00.000000 holonote-0.1.1a2/examples/basics/Basics.ipynb
+-rw-r--r--   0        0        0    16488 2020-02-02 00:00:00.000000 holonote-0.1.1a2/examples/basics/Basics_2D.ipynb
+-rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 holonote-0.1.1a2/examples/basics/MultiPlot.ipynb
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 holonote-0.1.1a2/examples/tutorial/00_Overview.ipynb
+-rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 holonote-0.1.1a2/examples/tutorial/01_First_Annotation.ipynb
+-rw-r--r--   0        0        0     5801 2020-02-02 00:00:00.000000 holonote-0.1.1a2/examples/tutorial/02_Multiple_Annotations.ipynb
+-rw-r--r--   0        0        0     8860 2020-02-02 00:00:00.000000 holonote-0.1.1a2/examples/tutorial/03_Styling_of_Annotations.ipynb
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 holonote-0.1.1a2/examples/tutorial/04_Make_an_App.ipynb
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 holonote-0.1.1a2/examples/tutorial/05_Watch_Events.ipynb
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 holonote-0.1.1a2/holonote/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 holonote-0.1.1a2/holonote/_version.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 holonote-0.1.1a2/holonote/_warnings.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 holonote-0.1.1a2/holonote/annotate/__init__.py
+-rw-r--r--   0        0        0    17152 2020-02-02 00:00:00.000000 holonote-0.1.1a2/holonote/annotate/annotator.py
+-rw-r--r--   0        0        0    18854 2020-02-02 00:00:00.000000 holonote-0.1.1a2/holonote/annotate/connector.py
+-rw-r--r--   0        0        0    20476 2020-02-02 00:00:00.000000 holonote-0.1.1a2/holonote/annotate/display.py
+-rw-r--r--   0        0        0    13288 2020-02-02 00:00:00.000000 holonote-0.1.1a2/holonote/annotate/table.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 holonote-0.1.1a2/holonote/annotate/typing.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 holonote-0.1.1a2/holonote/app/__init__.py
+-rw-r--r--   0        0        0    11583 2020-02-02 00:00:00.000000 holonote-0.1.1a2/holonote/app/panel.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 holonote-0.1.1a2/holonote/editor/__init__.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 holonote-0.1.1a2/holonote/editor/editors.py
+-rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 holonote-0.1.1a2/holonote/tests/conftest.py
+-rw-r--r--   0        0        0     7762 2020-02-02 00:00:00.000000 holonote-0.1.1a2/holonote/tests/test_annotation_table.py
+-rw-r--r--   0        0        0    13275 2020-02-02 00:00:00.000000 holonote-0.1.1a2/holonote/tests/test_annotators_advanced.py
+-rw-r--r--   0        0        0    17224 2020-02-02 00:00:00.000000 holonote-0.1.1a2/holonote/tests/test_annotators_basic.py
+-rw-r--r--   0        0        0     8170 2020-02-02 00:00:00.000000 holonote-0.1.1a2/holonote/tests/test_annotators_element.py
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 holonote-0.1.1a2/holonote/tests/test_annotators_interface.py
+-rw-r--r--   0        0        0     5487 2020-02-02 00:00:00.000000 holonote-0.1.1a2/holonote/tests/test_annotators_style.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 holonote-0.1.1a2/holonote/tests/test_app.py
+-rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 holonote-0.1.1a2/holonote/tests/test_connectors.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 holonote-0.1.1a2/holonote/tests/util.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 holonote-0.1.1a2/holonote/tests/benchmark/test_benchmarks.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 holonote-0.1.1a2/scripts/example_testing.py
+-rwxr-xr-x   0        0        0      191 2020-02-02 00:00:00.000000 holonote-0.1.1a2/scripts/conda/build.sh
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 holonote-0.1.1a2/scripts/conda/recipe/meta.yaml
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 holonote-0.1.1a2/scripts/jupyterlite/build.sh
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 holonote-0.1.1a2/scripts/jupyterlite/extra_packages.json
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 holonote-0.1.1a2/scripts/jupyterlite/jupyter-lite.json
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 holonote-0.1.1a2/scripts/jupyterlite/jupyter_lite_config.json
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 holonote-0.1.1a2/scripts/jupyterlite/package-lock.json
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 holonote-0.1.1a2/scripts/jupyterlite/package.json
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 holonote-0.1.1a2/scripts/jupyterlite/patch_lock.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 holonote-0.1.1a2/scripts/jupyterlite/update_lock.js
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 holonote-0.1.1a2/scripts/jupyterlite/files/Reset_Jupyterlite.ipynb
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 holonote-0.1.1a2/.gitignore
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 holonote-0.1.1a2/LICENSE.txt
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 holonote-0.1.1a2/README.md
+-rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 holonote-0.1.1a2/pyproject.toml
+-rw-r--r--   0        0        0     6403 2020-02-02 00:00:00.000000 holonote-0.1.1a2/PKG-INFO
```

### Comparing `holonote-0.1.1a1/.pre-commit-config.yaml` & `holonote-0.1.1a2/.pre-commit-config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # This is the configuration for pre-commit, a local framework for managing pre-commit hooks
 #   Check out the docs at: https://pre-commit.com/
 
 exclude: (\.min\.js$|\.svg$|\.html$)
 default_stages: [commit]
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: end-of-file-fixer
       - id: trailing-whitespace
       - id: mixed-line-ending
       - id: check-builtin-literals
       - id: check-case-conflict
       - id: check-docstring-first
       - id: check-executables-have-shebangs
       - id: check-toml
       - id: check-yaml
         exclude: scripts/conda/recipe/meta.yaml
       - id: check-json
       - id: detect-private-key
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.1.7
+    rev: v0.4.0
     hooks:
       - id: ruff
         files: holonote/
       - id: ruff-format
         files: holonote/
   - repo: https://github.com/hoxbro/clean_notebook
     rev: v0.1.14
@@ -34,10 +34,10 @@
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.6
     hooks:
     - id: codespell
       additional_dependencies:
         - tomli
   - repo: https://github.com/shellcheck-py/shellcheck-py
-    rev: "v0.9.0.6"
+    rev: "v0.10.0.1"
     hooks:
       - id: shellcheck
```

### Comparing `holonote-0.1.1a1/.github/workflows/build.yaml` & `holonote-0.1.1a2/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `holonote-0.1.1a1/.github/workflows/docs.yaml` & `holonote-0.1.1a2/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `holonote-0.1.1a1/.github/workflows/jupyterlite.yaml` & `holonote-0.1.1a2/.github/workflows/jupyterlite.yaml`

 * *Files identical despite different names*

### Comparing `holonote-0.1.1a1/.github/workflows/test.yaml` & `holonote-0.1.1a2/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `holonote-0.1.1a1/doc/conf.py` & `holonote-0.1.1a2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `holonote-0.1.1a1/doc/generate_modules.py` & `holonote-0.1.1a2/doc/generate_modules.py`

 * *Files identical despite different names*

### Comparing `holonote-0.1.1a1/doc/index.md` & `holonote-0.1.1a2/doc/index.md`

 * *Files identical despite different names*

### Comparing `holonote-0.1.1a1/doc/_static/assets/jupyterlite.svg` & `holonote-0.1.1a2/doc/_static/assets/jupyterlite.svg`

 * *Files identical despite different names*

### Comparing `holonote-0.1.1a1/doc/_static/css/custom.css` & `holonote-0.1.1a2/doc/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `holonote-0.1.1a1/doc/reference_manual/index.md` & `holonote-0.1.1a2/doc/reference_manual/index.md`

 * *Files identical despite different names*

### Comparing `holonote-0.1.1a1/doc/tutorial/index.md` & `holonote-0.1.1a2/doc/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `holonote-0.1.1a1/examples/assets/example.parquet` & `holonote-0.1.1a2/examples/assets/example.parquet`

 * *Files identical despite different names*

### Comparing `holonote-0.1.1a1/examples/basics/Basics.ipynb` & `holonote-0.1.1a2/examples/basics/Basics.ipynb`

 * *Files identical despite different names*

### Comparing `holonote-0.1.1a1/examples/basics/Basics_2D.ipynb` & `holonote-0.1.1a2/examples/basics/Basics_2D.ipynb`

 * *Files identical despite different names*

### Comparing `holonote-0.1.1a1/examples/basics/MultiPlot.ipynb` & `holonote-0.1.1a2/examples/basics/MultiPlot.ipynb`

 * *Files identical despite different names*

### Comparing `holonote-0.1.1a1/examples/tutorial/00_Overview.ipynb` & `holonote-0.1.1a2/examples/tutorial/00_Overview.ipynb`

 * *Files identical despite different names*

### Comparing `holonote-0.1.1a1/examples/tutorial/01_First_Annotation.ipynb` & `holonote-0.1.1a2/examples/tutorial/01_First_Annotation.ipynb`

 * *Files identical despite different names*

### Comparing `holonote-0.1.1a1/examples/tutorial/02_Multiple_Annotations.ipynb` & `holonote-0.1.1a2/examples/tutorial/02_Multiple_Annotations.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999600074404762%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(11, 'layout = raw_speed_curve + filt_speed_curve\\n'), (12, "*

 * *            "'layout')], delete: [11]}}, 3: {'source': {insert: [(3, 'annotator * layout')], "*

 * *            'delete: [3]}}}'}*

```diff
@@ -24,15 +24,16 @@
                 "raw_speed_data = pd.read_parquet(\"../assets/example.parquet\")\n",
                 "raw_speed_curve = raw_speed_data.hvplot(\"TIME\", \"SPEED\")\n",
                 "\n",
                 "filt_speed_data = raw_speed_data.copy()\n",
                 "filt_speed_data.loc[raw_speed_data.SPEED < 98, \"SPEED\"] = pd.NA\n",
                 "filt_speed_curve = filt_speed_data.hvplot(\"TIME\", \"SPEED\")\n",
                 "\n",
-                "raw_speed_curve + filt_speed_curve"
+                "layout = raw_speed_curve + filt_speed_curve\n",
+                "layout"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "5459593a-447d-4cc1-9a53-b22f791d23f5",
             "metadata": {},
             "source": [
@@ -49,15 +50,15 @@
             "id": "8197c71c-38c1-4752-b68d-b2866e783f53",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from holonote.annotate import Annotator\n",
                 "\n",
                 "annotator = Annotator(filt_speed_curve, fields=['description'])\n",
-                "annotator * raw_speed_curve + annotator * filt_speed_curve"
+                "annotator * layout"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "70543b07-eff9-4802-9884-b292c71bf5f3",
             "metadata": {},
             "source": [
```

### Comparing `holonote-0.1.1a1/examples/tutorial/03_Styling_of_Annotations.ipynb` & `holonote-0.1.1a2/examples/tutorial/03_Styling_of_Annotations.ipynb`

 * *Files identical despite different names*

### Comparing `holonote-0.1.1a1/examples/tutorial/04_Make_an_App.ipynb` & `holonote-0.1.1a2/examples/tutorial/05_Watch_Events.ipynb`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9418089110644258%*

 * *Differences: {"'cells'": "{0: {'id': 'fbba196f', 'source': {insert: [(0, '## Watch for events\\n'), (2, "*

 * *            '"It is possible to watch for events on a plot and trigger a callback when an event '*

 * *            'occurs.  This can be used to trigger a computation, or to update other plots or '*

 * *            "widgets. Here we'll show how to use it with [Panels](https://panel.holoviz.org) "*

 * *            'notifications. First, let\'s set up the annotations\\n")], delete: [4, 2, 1, 0]}}, 1: '*

 * *            "{'id': '86a4fefd- […]*

```diff
@@ -1,85 +1,74 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "29686db3-3167-44e4-8868-6b18b1e17ece",
+            "id": "fbba196f",
             "metadata": {},
             "source": [
-                "## Make an App\n",
+                "## Watch for events\n",
                 "\n",
-                "By using the rest of the HoloViz ecosystem, you can easily turn your annotated data into a fully interactive dashboard or web application.  Here we'll show how to use [Panel](https://panel.holoviz.org) to turn the annotated data into a dashboard that lets you explore the data and the annotations.\n",
-                "\n",
-                "But first, let's load the data:"
+                "It is possible to watch for events on a plot and trigger a callback when an event occurs.  This can be used to trigger a computation, or to update other plots or widgets. Here we'll show how to use it with [Panels](https://panel.holoviz.org) notifications. First, let's set up the annotations\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "e9254fc3-0447-440e-825e-68e02dcb9eb7",
+            "id": "86a4fefd-4aa9-476c-badc-b8ad0bcca9f4",
             "metadata": {},
             "outputs": [],
             "source": [
-                "import hvplot.pandas\n",
-                "import numpy as np\n",
-                "import pandas as pd\n",
+                "import holoviews as hv\n",
                 "import panel as pn\n",
                 "\n",
-                "pn.extension()\n",
-                "\n",
-                "speed_data = pd.read_parquet(\"../assets/example.parquet\")\n",
-                "speed_curve = speed_data.hvplot(\"TIME\", \"SPEED\")"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "e28ad0ab-b058-492e-a6e6-adb3bc5a497f",
-            "metadata": {},
-            "source": [
-                "To make the app more advanced we will add more fields to the data.  We'll add a `Stoppage` field that indicates whether it was a stoppage or not, and a `Reason` field that will contain the reason for the stoppage if it was a stoppage.  Lastly, we'll add a `Category` field that will contain the category of the event, which we later will set mechanical, electrical, planned, or other."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "74340a51-d1b0-4cd7-954f-923f45c50941",
-            "metadata": {},
-            "outputs": [],
-            "source": [
                 "from holonote.annotate import Annotator\n",
+                "from holonote.app import PanelWidgets\n",
+                "\n",
+                "hv.extension(\"bokeh\")\n",
+                "pn.extension(notifications=True)\n",
+                "\n",
+                "annotator = Annotator({\"x\": float}, fields=[\"description\"])\n",
+                "element = hv.Curve(range(10), kdims=\"x\")\n",
                 "\n",
-                "fields = [\"Stoppage\", \"Reason\", \"Category\"]\n",
-                "annotator = Annotator({\"TIME\": np.datetime64}, fields=fields)\n",
-                "annotator_element = annotator * speed_curve"
+                "tools = PanelWidgets(annotator)\n",
+                "pn.Row(tools, annotator * element)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "85ff1b48-ffb3-42e9-a9a4-c62ee239c12f",
+            "id": "63c6e452",
             "metadata": {},
             "source": [
-                "HoloNote has an easy to make the widgets to annotate the data in `PanelWidgets`, the options for the fields mentioned above will be passed to the `PanelWidgets` class with the `fields_values` dictionary. "
+                "With that being set up, we can now define a callback that will be triggered when the user add an annotation.  The callback will then display a simple notification.\n",
+                "\n",
+                "The argument to the callback is an event, which contains the following information:\n",
+                "- `type`: The type of event.\n",
+                "- `index`: The index of the annotation.\n",
+                "- `region`: The region that was added, updated, or deleted.\n",
+                "- `fields`: The fields that were added, updated, or deleted.\n",
+                "\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "b65b2e68-057c-490c-9061-4ee4ea69ca0e",
+            "id": "f9dfc126",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from holonote.app import PanelWidgets\n",
+                "def notification(event):\n",
+                "    if event.type == \"create\":\n",
+                "        pn.state.notifications.info(\"Annotation created\")\n",
+                "    elif event.type == \"delete\":\n",
+                "        pn.state.notifications.error(\"Annotation deleted\")\n",
+                "    elif event.type == \"update\":\n",
+                "        pn.state.notifications.success(\"Annotation updated\")\n",
                 "\n",
-                "fields_values = {\n",
-                "    \"Stoppage\": [\"Yes\", \"No\"],\n",
-                "    \"Category\": [\"Mechanical\", \"Electrical\", \"Planned\", \"Other\"],\n",
-                "}\n",
                 "\n",
-                "tools = PanelWidgets(annotator, field_values=fields_values)\n",
-                "pn.Row(tools, annotator_element).servable()"
+                "annotator.on_event(notification)"
             ]
         }
     ],
     "metadata": {
         "language_info": {
             "name": "python",
             "pygments_lexer": "ipython3"
```

### Comparing `holonote-0.1.1a1/holonote/__init__.py` & `holonote-0.1.1a2/holonote/__init__.py`

 * *Files identical despite different names*

### Comparing `holonote-0.1.1a1/holonote/_warnings.py` & `holonote-0.1.1a2/holonote/_warnings.py`

 * *Files identical despite different names*

### Comparing `holonote-0.1.1a1/holonote/annotate/annotator.py` & `holonote-0.1.1a2/holonote/annotate/annotator.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import holoviews as hv
 import pandas as pd
 import param
 
 from .._warnings import warn
 from .connector import Connector, SQLiteDB
-from .display import AnnotationDisplay, Indicator, Style  # noqa: F401
+from .display import AnnotationDisplay, Indicator, Style, _valid_element_opts  # noqa: F401
 from .table import AnnotationTable
 
 if TYPE_CHECKING:
     from .typing import SpecDict
 
 
 event_info = namedtuple("event_info", ["type", "index", "region", "fields"])
@@ -339,16 +339,48 @@
 
     def get_display(self, *kdims: str | hv.Dimension) -> AnnotationDisplay:
         element_key = tuple(map(str, kdims))
         if element_key not in self._displays:
             self._displays[element_key] = self._create_annotation_element(element_key)
         return self._displays[element_key]
 
-    def __mul__(self, other: hv.Element) -> hv.Overlay:
-        return other * self.get_element(*other.kdims)
+    def _get_kdims_from_other_element(self, other):
+        if isinstance(other, hv.DynamicMap):
+            if other.last is None:
+                hv.plotting.util.initialize_dynamic(other)
+            other = other.last
+        kdims = other.kdims
+        if not kdims or kdims == ["Element"]:
+            kdims = next(k for el in other.values() if (k := el.kdims))
+        kdims = [kdim for kdim in kdims if kdim.name in self.spec]
+        if kdims:
+            return kdims
+        else:
+            msg = "No valid kdims found in element"
+            raise ValueError(msg)
+
+    def __mul__(self, other: hv.Element | hv.Layout | hv.Overlay | hv.NdOverlay) -> hv.Overlay:
+        if isinstance(other, (hv.Overlay, hv.NdOverlay)):
+            kdims = self._get_kdims_from_other_element(other)
+            opts = other.opts.get().kwargs
+            return (other * self.get_element(*kdims)).opts(**opts)
+        elif isinstance(other, hv.Layout):
+            opts = other.opts.get().kwargs
+            to_layout = []
+            overlay_opts = _valid_element_opts()["Overlay"]
+            for el in other:
+                kdims = self._get_kdims_from_other_element(el)
+                el_opts = {k: v for k, v in el.opts.get().kwargs.items() if k in overlay_opts}
+                to_layout.append((el * self.get_element(*kdims)).opts(**el_opts))
+            layout = hv.Layout(to_layout).opts(**opts)
+            layout._max_cols = other._max_cols
+            return layout
+        else:
+            kdims = self._get_kdims_from_other_element(other)
+            return other * self.get_element(*kdims)
 
     def __rmul__(self, other: hv.Element) -> hv.Overlay:
         return self.__mul__(other)
 
     def refresh(self, clear=False) -> None:
         for v in self._displays.values():
             v._update_data()
```

### Comparing `holonote-0.1.1a1/holonote/annotate/connector.py` & `holonote-0.1.1a2/holonote/annotate/connector.py`

 * *Files identical despite different names*

### Comparing `holonote-0.1.1a1/holonote/annotate/display.py` & `holonote-0.1.1a2/holonote/annotate/display.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import weakref
-from functools import reduce
+from functools import cache, reduce
 from typing import TYPE_CHECKING, Any
 
 import colorcet as cc
 import holoviews as hv
 import numpy as np
 import param
 from bokeh.models.tools import BoxSelectTool, HoverTool, Tool
@@ -27,14 +27,21 @@
 _default_opts = {"apply_ranges": False, "show_legend": False}
 
 # Make red the first color
 _default_color = cc.palette["glasbey_category10"].copy()
 _default_color[:4] = [_default_color[3], *_default_color[:3]]
 
 
+@cache
+def _valid_element_opts():
+    if not hv.extension._loaded:
+        hv.extension("bokeh")
+    return hv.opts._element_keywords("bokeh")
+
+
 class Style(param.Parameterized):
     """
     Style class for controlling the appearance of the annotations
     indicator and editor.
 
     This can be accessed as an accessor on an annotator object,
     the following will set the annotation color to red:
@@ -66,17 +73,15 @@
         default=0.7, bounds=(0, 1), allow_refs=True, doc="Alpha value for selected regions"
     )
 
     edit_alpha = param.Number(
         default=0.4, bounds=(0, 1), allow_refs=True, doc="Alpha value for editing regions"
     )
 
-    color = param.Parameter(
-        default=hv.Cycle(_default_color), doc="Color of the indicator", allow_refs=True
-    )
+    color = param.Parameter(default=None, doc="Color of the indicator", allow_refs=True)
     edit_color = param.Parameter(default="blue", doc="Color of the editor", allow_refs=True)
     selection_color = param.Parameter(
         default=None, doc="Color of selection, by the default the same as color", allow_refs=True
     )
 
     # Indicator opts (default and selection)
     opts = _StyleOpts(default={})
@@ -86,27 +91,46 @@
 
     # Editor opts
     edit_opts = _StyleOpts(default={"line_color": "black"})
     edit_line_opts = _StyleOpts(default={})
     edit_span_opts = _StyleOpts(default={})
     edit_rectangle_opts = _StyleOpts(default={})
 
+    _groupby = ()
+    _colormap = None
+
+    @property
+    def _color(self):
+        if self.color is None:
+            if self._groupby:
+                # This is the main point of this method
+                # we use this to be able to memorize the colormap
+                # so the color are the same no matter what
+                # the order of the groupby is
+                dim = hv.dim(self._groupby[0])
+                self._colormap = dict(zip(self._groupby[1], _default_color))
+                return dim.categorize(self._colormap)
+            else:
+                return _default_color[0]
+
+        return self.color
+
     @property
     def _indicator_selection(self) -> dict[str, tuple]:
         select = {"alpha": (self.selection_alpha, self.alpha)}
         if self.selection_color is not None:
-            if isinstance(self.color, hv.dim):
-                msg = "'Style.color' cannot be a `hv.dim` when 'Style.selection_color' is not None"
+            if isinstance(self._color, hv.dim):
+                msg = "'Style.color' cannot be a `hv.dim` / `None` when 'Style.selection_color' is not None"
                 raise ValueError(msg)
             else:
-                select["color"] = (self.selection_color, self.color)
+                select["color"] = (self.selection_color, self._color)
         return select
 
     def indicator(self, **select_opts) -> tuple[hv.Options, ...]:
-        opts = {**_default_opts, "color": self.color, **select_opts, **self.opts}
+        opts = {**_default_opts, "color": self._color, **select_opts, **self.opts}
         return (
             hv.opts.Rectangles(**opts, **self.rectangle_opts),
             hv.opts.VSpans(**opts, **self.span_opts),
             hv.opts.HSpans(**opts, **self.span_opts),
             hv.opts.VLines(**opts, **self.line_opts),
             hv.opts.HLines(**opts, **self.line_opts),
         )
@@ -123,14 +147,15 @@
             hv.opts.VSpan(**opts, **self.edit_span_opts),
             hv.opts.HSpan(**opts, **self.edit_span_opts),
             hv.opts.VLine(**opts, **self.edit_line_opts),
             hv.opts.HLine(**opts, **self.edit_line_opts),
         )
 
     def reset(self) -> None:
+        self._colormap = None
         params = self.param.objects().items()
         self.param.update(**{k: v.default for k, v in params if k != "name"})
 
 
 class Indicator:
     """
     Collection of class methods that express annotation data as final
@@ -242,20 +267,34 @@
 
     def _set_region_format(self) -> None:
         self.region_format = "-".join([self.annotator.spec[k]["region"] for k in self.kdims])
 
     def _update_data(self):
         with param.edit_constant(self):
             self.data = self.annotator.get_dataframe(dims=self.kdims)
+        if self.annotator.groupby:
+            self.annotator.style._groupby = (
+                self.annotator.groupby,
+                sorted(self.data[self.annotator.groupby].unique()),
+            )
 
     @property
     def element(self):
         return self.overlay()
 
     @property
+    def edit_streams(self) -> dict[str, hv.streams.Stream]:
+        edit_streams = {}
+        if self.region_format in ("range", "range-range"):
+            edit_streams["box_select"] = self._edit_streams[0]
+        elif self.region_format in ("point", "point-point"):
+            edit_streams["tap"] = self._edit_streams[1]
+        return edit_streams
+
+    @property
     def edit_tools(self) -> list[Tool]:
         tools = []
         if self.region_format == "range":
             tools.append(BoxSelectTool(dimensions="width"))
         elif self.region_format == "range-range":
             tools.append(BoxSelectTool())
         elif self.region_format == "point":
@@ -263,15 +302,15 @@
         elif self.region_format == "point-point":
             tools.append("tap")
         return tools
 
     @classmethod
     def _infer_kdim_dtypes(cls, element):
         if not isinstance(element, hv.Element):
-            msg = "Supplied object {element} is not a bare HoloViews Element"
+            msg = f"Supplied object {element} is not a bare HoloViews Element"
             raise ValueError(msg)
         kdim_dtypes = {}
         for kdim in element.dimensions(selection="key"):
             kdim_dtypes[str(kdim)] = type(element.dimension_values(kdim)[0])
         return kdim_dtypes
 
     def clear_indicated_region(self):
@@ -294,30 +333,31 @@
     @property
     def selection_enabled(self) -> bool:
         return self._selection_enabled
 
     @selection_enabled.setter
     def selection_enabled(self, enabled: bool) -> None:
         self._selection_enabled = enabled
+        if not enabled:
+            self.clear_indicated_region()
 
     @property
     def editable_enabled(self) -> bool:
         return self._editable_enabled
 
     @editable_enabled.setter
     def editable_enabled(self, enabled: bool) -> None:
         self._editable_enabled = enabled
-        if not enabled:
-            self.clear_indicated_region()
 
     def _filter_stream_values(self, bounds, x, y, geometry):
         if not self._editable_enabled:
             return (None, None, None, None)
         if self.region_format == "point" and bounds:
-            x = (bounds[0] + bounds[2]) / 2
+            #  x is calculated this way to handle datetime
+            x = bounds[0] + (bounds[2] - bounds[0]) / 2
             y = None
             bounds = (x, 0, x, 0)
         elif "range" not in self.region_format:
             bounds = None
 
         # If selection enabled, tap stream used for selection not for creating point regions
         # if ('point' in self.region_format and self.selection_enabled) or 'point' not in self.region_format:
@@ -397,24 +437,24 @@
             inputs = {str(k): v for k, v in zip(self.kdims, (x, y))}
             indices = self.get_indices_by_position(**inputs)
             if indices:
                 self.annotator.select_by_index(indices[0])
             else:
                 self.annotator.select_by_index()
 
-        tap_stream = hv.streams.Tap(source=element, transient=True)
-        tap_stream.add_subscriber(tap_selector)
+        self._tap_stream = hv.streams.Tap(source=element, transient=True)
+        self._tap_stream.add_subscriber(tap_selector)
         return element
 
     def register_double_tap_clear(self, element: hv.Element) -> hv.Element:
         def double_tap_clear(x, y):
             self.clear_indicated_region()
 
-        double_tap_stream = hv.streams.DoubleTap(source=element, transient=True)
-        double_tap_stream.add_subscriber(double_tap_clear)
+        self._double_tap_stream = hv.streams.DoubleTap(source=element, transient=True)
+        self._double_tap_stream.add_subscriber(double_tap_clear)
         return element
 
     def indicators(self) -> hv.DynamicMap:
         if not hasattr(self, "_indicators"):
             self.register_tap_selector(self._element)
             self.register_double_tap_clear(self._element)
```

### Comparing `holonote-0.1.1a1/holonote/annotate/table.py` & `holonote-0.1.1a2/holonote/annotate/table.py`

 * *Files identical despite different names*

### Comparing `holonote-0.1.1a1/holonote/tests/conftest.py` & `holonote-0.1.1a2/holonote/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `holonote-0.1.1a1/holonote/tests/test_annotation_table.py` & `holonote-0.1.1a2/holonote/tests/test_annotation_table.py`

 * *Files identical despite different names*

### Comparing `holonote-0.1.1a1/holonote/tests/test_annotators_advanced.py` & `holonote-0.1.1a2/holonote/tests/test_annotators_advanced.py`

 * *Files identical despite different names*

### Comparing `holonote-0.1.1a1/holonote/tests/test_annotators_basic.py` & `holonote-0.1.1a2/holonote/tests/test_annotators_basic.py`

 * *Files identical despite different names*

### Comparing `holonote-0.1.1a1/holonote/tests/test_annotators_element.py` & `holonote-0.1.1a2/holonote/tests/test_annotators_element.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import holoviews as hv
 import pytest
+from holoviews.operation.datashader import rasterize
 
 from holonote.tests.util import get_editor, get_indicator
 
 
 def get_editor_data(annotator, element_type, kdims=None):
     el = get_editor(annotator, element_type, kdims)
     return getattr(el, "data", None)
@@ -42,14 +43,23 @@
     expected1 = [-0.25, 0.25]
     assert output1 == expected1
     output2 = output.iloc[0]["description"]
     expected2 = "Test"
     assert output2 == expected2
 
 
+def test_edit_streams(annotator_range1d) -> None:
+    annotator = annotator_range1d
+    edit_streams = annotator.get_display("TIME").edit_streams
+    assert len(edit_streams) == 1
+    assert "box_select" in edit_streams
+    assert "tap" not in edit_streams
+    assert "lasso_select" not in edit_streams
+
+
 def test_set_regions_range2d(annotator_range2d) -> None:
     annotator = annotator_range2d
     annotator.get_display("x", "y")
 
     # No regions has been set
     output = get_editor_data(annotator, hv.Rectangles)
     assert output.empty
@@ -178,7 +188,74 @@
     iter_indicator = get_indicator(cat_annotator, hv.VSpans)
     indicator = next(iter_indicator)
     assert indicator.data.shape == (2, 5)
     assert (indicator.data["category"] == "A").all()
 
     with pytest.raises(StopIteration):
         next(iter_indicator)
+
+
+def test_multiply_overlay(annotator_range1d):
+    el1 = hv.Curve([], kdims=["TIME"])
+    el2 = hv.Curve([], kdims=["TIME"])
+    el = el1 * el2
+    assert isinstance(el, hv.Overlay)
+
+    el = el * annotator_range1d
+    hv.render(el)
+    assert isinstance(el.last, hv.Overlay)
+
+    el.opts(width=100)
+    hv.render(el)
+    assert el.last.opts.get().kwargs.get("width") == 100
+
+
+def test_multiply_ndoverlay(annotator_range1d):
+    el1 = hv.Curve([], kdims=["TIME"])
+    el2 = hv.Curve([], kdims=["TIME"])
+    el = hv.NdOverlay({1: el1, 2: el2})
+    assert isinstance(el, hv.NdOverlay)
+
+    el = el * annotator_range1d
+    hv.render(el)
+    assert isinstance(el.last, hv.Overlay)
+
+    el.opts(width=100)
+    hv.render(el)
+    assert el.last.opts.get().kwargs.get("width") == 100
+
+
+def test_multiply_layout(annotator_range1d):
+    el1 = hv.Curve([], kdims=["TIME"])
+    el2 = hv.Curve([], kdims=["TIME"])
+    el = el1 + el2
+    assert isinstance(el, hv.Layout)
+
+    el = el * annotator_range1d
+    hv.render(el)
+    assert isinstance(el, hv.Layout)
+
+    el.opts(width=100)
+    hv.render(el)
+    assert el.opts.get().kwargs.get("width") == 100
+
+
+def test_multiply_dynamicmap(annotator_range1d):
+    # rasterize creates a dynamicmap
+    el1 = rasterize(hv.Curve([], kdims=["TIME"]))
+    assert isinstance(el1, hv.DynamicMap)
+
+    el = el1 * annotator_range1d
+    hv.render(el)
+    # an overlay including a dynamicmap is still a dynamicmap
+    assert isinstance(el, hv.DynamicMap)
+
+
+def test_multiply_dynamicmap_layout(annotator_range1d):
+    el1 = rasterize(hv.Curve([], kdims=["TIME"]))
+    el2 = hv.Curve([], kdims=["TIME"])
+    el = el1 + el2
+    assert isinstance(el, hv.Layout)
+
+    el = el * annotator_range1d
+    hv.render(el)
+    assert isinstance(el, hv.Layout)
```

### Comparing `holonote-0.1.1a1/holonote/tests/test_annotators_interface.py` & `holonote-0.1.1a2/holonote/tests/test_annotators_interface.py`

 * *Files identical despite different names*

### Comparing `holonote-0.1.1a1/holonote/tests/test_annotators_style.py` & `holonote-0.1.1a2/holonote/tests/test_annotators_style.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import holoviews as hv
 import pandas as pd
 import pytest
 
 from holonote.annotate import Style
+from holonote.annotate.display import _default_color
 from holonote.tests.util import get_editor, get_indicator
 
 
 def compare_indicator_color(indicator, style):
     if isinstance(indicator.opts["color"], hv.dim):
         if isinstance(style.color, hv.dim):
             assert str(indicator.opts["color"]) == str(style.color)
+        elif style.color is None and style._colormap:
+            assert dict(zip(style._groupby[1], _default_color)) == style._colormap
         else:
-            style_color = (
-                style.color.values[0] if isinstance(style.color, hv.Cycle) else style.color
-            )
             expected_dim = hv.dim("__selected__").categorize(
-                categories={True: style.selection_color}, default=style_color
+                categories={True: style.selection_color}, default=style.color
             )
             assert str(indicator.opts["color"]) == str(expected_dim)
     else:
         assert indicator.opts["color"] == style.color
 
 
 def compare_style(cat_annotator):
@@ -82,14 +82,17 @@
     style = cat_annotator.style
     style.color = hv.dim("category").categorize(
         categories={"B": "red", "A": "blue", "C": "green"}, default="grey"
     )
     compare_style(cat_annotator)
 
 
+@pytest.mark.xfail(
+    reason="hv.dim is not supported for selection.color in the current implementation"
+)
 def test_style_selection_color(cat_annotator):
     style = cat_annotator.style
     style.selection_color = "blue"
     compare_style(cat_annotator)
     sel_data = get_selected_indicator_data(cat_annotator)
     assert sel_data.sum() == 0
 
@@ -110,15 +113,15 @@
 
 def test_style_error_color_dim_and_selection(cat_annotator):
     style = cat_annotator.style
     style.color = hv.dim("category").categorize(
         categories={"B": "red", "A": "blue", "C": "green"}, default="grey"
     )
     style.selection_color = "blue"
-    msg = r"'Style\.color' cannot be a `hv.dim` when 'Style.selection_color' is not None"
+    msg = "'Style.color' cannot be a `hv.dim` / `None` when 'Style.selection_color' is not None"
     with pytest.raises(ValueError, match=msg):
         compare_style(cat_annotator)
 
 
 def test_style_opts(cat_annotator):
     cat_annotator.style.opts = {"line_width": 2}
     compare_style(cat_annotator)
@@ -153,10 +156,10 @@
 
 
 def test_groupby_color_change(cat_annotator) -> None:
     cat_annotator.groupby = "category"
     cat_annotator.visible = ["A", "B", "C"]
 
     indicators = hv.render(cat_annotator.get_display("x").static_indicators()).renderers
-    color_cycle = cat_annotator.style.color.values
+    color_cycle = cat_annotator.style._colormap.values()
     for indicator, expected_color in zip(indicators, color_cycle):
         assert indicator.glyph.fill_color == expected_color
```

### Comparing `holonote-0.1.1a1/holonote/tests/test_connectors.py` & `holonote-0.1.1a2/holonote/tests/test_connectors.py`

 * *Files identical despite different names*

### Comparing `holonote-0.1.1a1/holonote/tests/util.py` & `holonote-0.1.1a2/holonote/tests/util.py`

 * *Files identical despite different names*

### Comparing `holonote-0.1.1a1/holonote/tests/benchmark/test_benchmarks.py` & `holonote-0.1.1a2/holonote/tests/benchmark/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `holonote-0.1.1a1/scripts/example_testing.py` & `holonote-0.1.1a2/scripts/example_testing.py`

 * *Files identical despite different names*

### Comparing `holonote-0.1.1a1/scripts/conda/recipe/meta.yaml` & `holonote-0.1.1a2/scripts/conda/recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `holonote-0.1.1a1/scripts/jupyterlite/patch_lock.py` & `holonote-0.1.1a2/scripts/jupyterlite/patch_lock.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,16 +10,20 @@
     with open(file_path, "rb") as file:
         for byte_block in iter(lambda: file.read(4096), b""):
             sha256_hash.update(byte_block)
 
     return sha256_hash.hexdigest()
 
 
+with open("package.json") as f:
+    package = json.load(f)
+pyodide_version = package["dependencies"]["pyodide"].removeprefix("^")
+
 path = "pyodide-lock.json"
-url = "https://cdn.jsdelivr.net/pyodide/v0.24.1/full"
+url = f"https://cdn.jsdelivr.net/pyodide/v{pyodide_version}/full"
 
 with open(path) as f:
     data = json.load(f)
 
 for p in data["packages"].values():
     if not p["file_name"].startswith("http"):
         p["file_name"] = os.path.join(url, p["file_name"])
```

### Comparing `holonote-0.1.1a1/LICENSE.txt` & `holonote-0.1.1a2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `holonote-0.1.1a1/README.md` & `holonote-0.1.1a2/README.md`

 * *Files identical despite different names*

### Comparing `holonote-0.1.1a1/pyproject.toml` & `holonote-0.1.1a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     "pre-commit",
     "setuptools_scm",
     "pytest",
     "nbval",
     "hvplot",
     "fastparquet",
     "scipy",
+    "datashader",
+    "dask[dataframe]",
 ]
 examples = [
     "holonote[dev]",
     "jupyterlab",
     "jupyterlab-myst",
 ]
```

### Comparing `holonote-0.1.1a1/PKG-INFO` & `holonote-0.1.1a2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: holonote
-Version: 0.1.1a1
+Version: 0.1.1a2
 Summary: Annotate your data
 License: Copyright (c) 2023, HoloViz team (holoviz.org).
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are
         met:
@@ -39,25 +39,35 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Requires-Dist: holoviews>=1.18.0
 Requires-Dist: pandas
 Provides-Extra: dev
+Requires-Dist: dask[dataframe]; extra == 'dev'
+Requires-Dist: datashader; extra == 'dev'
 Requires-Dist: fastparquet; extra == 'dev'
 Requires-Dist: hvplot; extra == 'dev'
 Requires-Dist: nbval; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: scipy; extra == 'dev'
 Requires-Dist: setuptools-scm; extra == 'dev'
 Provides-Extra: examples
-Requires-Dist: holonote[dev]; extra == 'examples'
+Requires-Dist: dask[dataframe]; extra == 'examples'
+Requires-Dist: datashader; extra == 'examples'
+Requires-Dist: fastparquet; extra == 'examples'
+Requires-Dist: hvplot; extra == 'examples'
 Requires-Dist: jupyterlab; extra == 'examples'
 Requires-Dist: jupyterlab-myst; extra == 'examples'
+Requires-Dist: nbval; extra == 'examples'
+Requires-Dist: pre-commit; extra == 'examples'
+Requires-Dist: pytest; extra == 'examples'
+Requires-Dist: scipy; extra == 'examples'
+Requires-Dist: setuptools-scm; extra == 'examples'
 Description-Content-Type: text/markdown
 
 # `holonote`
 
 The `holonote` library offers tools to create, edit and persist
 annotated regions for [HoloViews](https://holoviews.org/).
```

