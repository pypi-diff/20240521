# Comparing `tmp/apluggy-1.0.0.tar.gz` & `tmp/apluggy-1.0.1.tar.gz`

## Comparing `apluggy-1.0.0.tar` & `apluggy-1.0.1.tar`

### file list

```diff
@@ -1,60 +1,65 @@
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 apluggy-1.0.0/setup.cfg
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 apluggy-1.0.0/.github/release.yml
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 apluggy-1.0.0/.github/workflows/pypi.yml
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 apluggy-1.0.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 apluggy-1.0.0/.github/workflows/type-check.yml
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 apluggy-1.0.0/.github/workflows/unit-test.yml
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 apluggy-1.0.0/.vscode/settings.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 apluggy-1.0.0/src/apluggy/__about__.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 apluggy-1.0.0/src/apluggy/__init__.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 apluggy-1.0.0/src/apluggy/_decorator.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 apluggy-1.0.0/src/apluggy/stack/__init__.py
--rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 apluggy-1.0.0/src/apluggy/stack/aexit.py
--rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 apluggy-1.0.0/src/apluggy/stack/async_.py
--rw-r--r--   0        0        0     4692 2020-02-02 00:00:00.000000 apluggy-1.0.0/src/apluggy/stack/sync.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 apluggy-1.0.0/src/apluggy/stack/types.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 apluggy-1.0.0/src/apluggy/wrap/__init__.py
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 apluggy-1.0.0/src/apluggy/wrap/ext.py
--rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 apluggy-1.0.0/src/apluggy/wrap/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/test_decorator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/plugins/__init__.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/plugins/module_plugin.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/plugins/spec.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/plugins/test_call.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/aexit/__init__.py
--rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/aexit/test_aexit.py
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/aexit/test_demo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/async/__init__.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/async/exc.py
--rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/async/runner.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/async/test_imp.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/async/test_refs.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/async/test_runner.py
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/async/test_single.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/async/refs/__init__.py
--rw-r--r--   0        0        0     6798 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/async/refs/dunder.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/async/refs/exit_.py
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/async/refs/nested.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/async/refs/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/sync/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/sync/exc.py
--rw-r--r--   0        0        0     4983 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/sync/runner.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/sync/test_imp.py
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/sync/test_refs.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/sync/test_single.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/sync/refs/__init__.py
--rw-r--r--   0        0        0     4829 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/sync/refs/dunder.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/sync/refs/exit_.py
--rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/sync/refs/nested.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/stack/sync/refs/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/test/__init__.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/utils/probe.py
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 apluggy-1.0.0/tests/utils/st.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 apluggy-1.0.0/.gitignore
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 apluggy-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0     8366 2020-02-02 00:00:00.000000 apluggy-1.0.0/README.md
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 apluggy-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     9559 2020-02-02 00:00:00.000000 apluggy-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 apluggy-1.0.1/setup.cfg
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 apluggy-1.0.1/.github/dependabot.yml
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 apluggy-1.0.1/.github/release.yml
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 apluggy-1.0.1/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 apluggy-1.0.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 apluggy-1.0.1/.github/workflows/type-check.yml
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 apluggy-1.0.1/.github/workflows/unit-test-latest.yml
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 apluggy-1.0.1/.github/workflows/unit-test-min.yml
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 apluggy-1.0.1/.github/workflows/unit-test.yml
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 apluggy-1.0.1/.vscode/settings.json
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 apluggy-1.0.1/ci/latest/requirements.txt
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 apluggy-1.0.1/ci/minimum/requirements.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 apluggy-1.0.1/src/apluggy/__about__.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 apluggy-1.0.1/src/apluggy/__init__.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 apluggy-1.0.1/src/apluggy/_decorator.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 apluggy-1.0.1/src/apluggy/stack/__init__.py
+-rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 apluggy-1.0.1/src/apluggy/stack/aexit.py
+-rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 apluggy-1.0.1/src/apluggy/stack/async_.py
+-rw-r--r--   0        0        0     4692 2020-02-02 00:00:00.000000 apluggy-1.0.1/src/apluggy/stack/sync.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 apluggy-1.0.1/src/apluggy/stack/types.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 apluggy-1.0.1/src/apluggy/wrap/__init__.py
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 apluggy-1.0.1/src/apluggy/wrap/ext.py
+-rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 apluggy-1.0.1/src/apluggy/wrap/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/test_decorator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/plugins/__init__.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/plugins/module_plugin.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/plugins/spec.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/plugins/test_call.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/stack/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/stack/aexit/__init__.py
+-rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/stack/aexit/test_aexit.py
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/stack/aexit/test_demo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/stack/async/__init__.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/stack/async/exc.py
+-rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/stack/async/runner.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/stack/async/test_imp.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/stack/async/test_refs.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/stack/async/test_runner.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/stack/async/test_single.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/stack/async/refs/__init__.py
+-rw-r--r--   0        0        0     6798 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/stack/async/refs/dunder.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/stack/async/refs/exit_.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/stack/async/refs/nested.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/stack/async/refs/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/stack/sync/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/stack/sync/exc.py
+-rw-r--r--   0        0        0     4983 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/stack/sync/runner.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/stack/sync/test_imp.py
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/stack/sync/test_refs.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/stack/sync/test_single.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/stack/sync/refs/__init__.py
+-rw-r--r--   0        0        0     4829 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/stack/sync/refs/dunder.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/stack/sync/refs/exit_.py
+-rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/stack/sync/refs/nested.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/stack/sync/refs/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/test/__init__.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/utils/probe.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 apluggy-1.0.1/tests/utils/st.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 apluggy-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 apluggy-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     8366 2020-02-02 00:00:00.000000 apluggy-1.0.1/README.md
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 apluggy-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     9559 2020-02-02 00:00:00.000000 apluggy-1.0.1/PKG-INFO
```

### Comparing `apluggy-1.0.0/.github/workflows/pypi.yml` & `apluggy-1.0.1/.github/workflows/pypi.yml`

 * *Files 19% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 jobs:
   deploy:
     runs-on: ubuntu-latest
     environment: pypi
     permissions:
       id-token: write
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: '3.10'
 
       - name: Install packages
         run: |
           pip install --upgrade pip
           pip install --upgrade hatch
```

### Comparing `apluggy-1.0.0/.github/workflows/release.yml` & `apluggy-1.0.1/.github/workflows/release.yml`

 * *Files 22% similar despite different names*

```diff
@@ -9,17 +9,17 @@
   deploy:
     runs-on: ubuntu-latest
     permissions:
       contents: write
 
     steps:
       - name: Checkout
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
       - name: Install gh CLI
-        uses: actions/setup-node@v3
+        uses: actions/setup-node@v4
         with:
           node-version: "18"
       - name: Create Release
         env:
           GH_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         run: |
           gh release create ${GITHUB_REF#refs/tags/} \
```

### Comparing `apluggy-1.0.0/.github/workflows/type-check.yml` & `apluggy-1.0.1/.github/workflows/type-check.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 name: Check static types
 
 on:
   push:
     branches:
-      - "**"
+      - main
   pull_request:
     branches:
-      - "**"
+      - main
 
 jobs:
   run:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.10"
 
       - name: Install packages
         run: |
           pip install --upgrade pip
           pip install --use-pep517 -e '.[tests]'
```

### Comparing `apluggy-1.0.0/.github/workflows/unit-test.yml` & `apluggy-1.0.1/.github/workflows/unit-test.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 name: Run unit tests
 
 on:
   push:
     branches:
-      - "**"
+      - main
   pull_request:
     branches:
-      - "**"
+      - main
 
 concurrency:
   group: unit-test-${{ github.head_ref }}
   cancel-in-progress: true
 
 env:
   PYTHONUNBUFFERED: "1"
@@ -23,30 +23,30 @@
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, macos-latest]
         python-version: ["3.10", "3.11", "3.12"]
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install packages
         run: |
           pip install --upgrade pip
-          pip install --use-pep517 -e '.[tests]'
+          pip install -e '.[tests]'
           pip list
 
       - name: Run tests
         run: pytest -vv --cov --cov-report=xml
 
       - name: Upload coverage to Codecov
         if: matrix.os == 'ubuntu-latest'
-        uses: codecov/codecov-action@v1
+        uses: codecov/codecov-action@v4
         with:
           fail_ci_if_error: true
           token: ${{ secrets.CODECOV_TOKEN }}
           verbose: true
```

### Comparing `apluggy-1.0.0/src/apluggy/_decorator.py` & `apluggy-1.0.1/src/apluggy/_decorator.py`

 * *Files identical despite different names*

### Comparing `apluggy-1.0.0/src/apluggy/stack/aexit.py` & `apluggy-1.0.1/src/apluggy/stack/aexit.py`

 * *Files identical despite different names*

### Comparing `apluggy-1.0.0/src/apluggy/stack/async_.py` & `apluggy-1.0.1/src/apluggy/stack/async_.py`

 * *Files identical despite different names*

### Comparing `apluggy-1.0.0/src/apluggy/stack/sync.py` & `apluggy-1.0.1/src/apluggy/stack/sync.py`

 * *Files identical despite different names*

### Comparing `apluggy-1.0.0/src/apluggy/wrap/ext.py` & `apluggy-1.0.1/src/apluggy/wrap/ext.py`

 * *Files identical despite different names*

### Comparing `apluggy-1.0.0/src/apluggy/wrap/main.py` & `apluggy-1.0.1/src/apluggy/wrap/main.py`

 * *Files identical despite different names*

### Comparing `apluggy-1.0.0/tests/test_decorator.py` & `apluggy-1.0.1/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `apluggy-1.0.0/tests/plugins/test_call.py` & `apluggy-1.0.1/tests/plugins/test_call.py`

 * *Files identical despite different names*

### Comparing `apluggy-1.0.0/tests/stack/aexit/test_aexit.py` & `apluggy-1.0.1/tests/stack/aexit/test_aexit.py`

 * *Files identical despite different names*

### Comparing `apluggy-1.0.0/tests/stack/aexit/test_demo.py` & `apluggy-1.0.1/tests/stack/aexit/test_demo.py`

 * *Files identical despite different names*

### Comparing `apluggy-1.0.0/tests/stack/async/runner.py` & `apluggy-1.0.1/tests/stack/async/runner.py`

 * *Files identical despite different names*

### Comparing `apluggy-1.0.0/tests/stack/async/test_imp.py` & `apluggy-1.0.1/tests/stack/async/test_imp.py`

 * *Files identical despite different names*

### Comparing `apluggy-1.0.0/tests/stack/async/test_refs.py` & `apluggy-1.0.1/tests/stack/async/test_refs.py`

 * *Files identical despite different names*

### Comparing `apluggy-1.0.0/tests/stack/async/test_runner.py` & `apluggy-1.0.1/tests/stack/async/test_runner.py`

 * *Files identical despite different names*

### Comparing `apluggy-1.0.0/tests/stack/async/test_single.py` & `apluggy-1.0.1/tests/stack/async/test_single.py`

 * *Files identical despite different names*

### Comparing `apluggy-1.0.0/tests/stack/async/refs/dunder.py` & `apluggy-1.0.1/tests/stack/async/refs/dunder.py`

 * *Files identical despite different names*

### Comparing `apluggy-1.0.0/tests/stack/async/refs/exit_.py` & `apluggy-1.0.1/tests/stack/async/refs/exit_.py`

 * *Files identical despite different names*

### Comparing `apluggy-1.0.0/tests/stack/async/refs/nested.py` & `apluggy-1.0.1/tests/stack/async/refs/nested.py`

 * *Files identical despite different names*

### Comparing `apluggy-1.0.0/tests/stack/sync/runner.py` & `apluggy-1.0.1/tests/stack/sync/runner.py`

 * *Files identical despite different names*

### Comparing `apluggy-1.0.0/tests/stack/sync/test_imp.py` & `apluggy-1.0.1/tests/stack/sync/test_imp.py`

 * *Files identical despite different names*

### Comparing `apluggy-1.0.0/tests/stack/sync/test_refs.py` & `apluggy-1.0.1/tests/stack/sync/test_refs.py`

 * *Files identical despite different names*

### Comparing `apluggy-1.0.0/tests/stack/sync/test_single.py` & `apluggy-1.0.1/tests/stack/sync/test_single.py`

 * *Files identical despite different names*

### Comparing `apluggy-1.0.0/tests/stack/sync/refs/dunder.py` & `apluggy-1.0.1/tests/stack/sync/refs/dunder.py`

 * *Files identical despite different names*

### Comparing `apluggy-1.0.0/tests/stack/sync/refs/nested.py` & `apluggy-1.0.1/tests/stack/sync/refs/nested.py`

 * *Files identical despite different names*

### Comparing `apluggy-1.0.0/tests/utils/probe.py` & `apluggy-1.0.1/tests/utils/probe.py`

 * *Files identical despite different names*

### Comparing `apluggy-1.0.0/tests/utils/st.py` & `apluggy-1.0.1/tests/utils/st.py`

 * *Files identical despite different names*

### Comparing `apluggy-1.0.0/.gitignore` & `apluggy-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `apluggy-1.0.0/LICENSE.txt` & `apluggy-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apluggy-1.0.0/README.md` & `apluggy-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `apluggy-1.0.0/pyproject.toml` & `apluggy-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
-  "pluggy>=1.0",
+  "pluggy>=1.3",
   "decorator>=5.1",
   "types-decorator>=5.1",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 tests = [
```

### Comparing `apluggy-1.0.0/PKG-INFO` & `apluggy-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: apluggy
-Version: 1.0.0
+Version: 1.0.1
 Summary: A wrapper of "pluggy" to support asyncio and context managers
 Project-URL: Documentation, https://github.com/simonsobs/apluggy#readme
 Project-URL: Issues, https://github.com/simonsobs/apluggy/issues
 Project-URL: Source, https://github.com/simonsobs/apluggy
 Author-email: Tai Sakuma <tai.sakuma@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -13,15 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Requires-Dist: decorator>=5.1
-Requires-Dist: pluggy>=1.0
+Requires-Dist: pluggy>=1.3
 Requires-Dist: types-decorator>=5.1
 Provides-Extra: tests
 Requires-Dist: hypothesis>=6.68; extra == 'tests'
 Requires-Dist: pytest-asyncio>=0.18; extra == 'tests'
 Requires-Dist: pytest-cov>=3.0; extra == 'tests'
 Requires-Dist: pytest-timeout>=2.1; extra == 'tests'
 Requires-Dist: pytest>=7.0; extra == 'tests'
```

