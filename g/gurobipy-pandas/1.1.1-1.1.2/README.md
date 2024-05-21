# Comparing `tmp/gurobipy_pandas-1.1.1.tar.gz` & `tmp/gurobipy_pandas-1.1.2.tar.gz`

## Comparing `gurobipy_pandas-1.1.1.tar` & `gurobipy_pandas-1.1.2.tar`

### file list

```diff
@@ -1,66 +1,64 @@
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/.readthedocs.yaml
--rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/Makefile
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/tox.ini
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/.github/workflows/build-wheel.yml
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/.github/workflows/code-quality.yml
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/.github/workflows/notebook-examples.yml
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/.github/workflows/publish-pypi.yml
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/.github/workflows/release.yml
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/.github/workflows/test-wheel.yml
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/.github/workflows/unit-tests.yml
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/docs/make.bat
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/docs/requirements-examples.txt
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/docs/requirements.txt
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/docs/source/acknowledgements.rst
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/docs/source/advanced.rst
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/docs/source/api.rst
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/docs/source/conf.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/docs/source/contact.rst
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/docs/source/examples.rst
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/docs/source/index.rst
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/docs/source/installation.rst
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/docs/source/license.rst
--rw-r--r--   0        0        0     6209 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/docs/source/naming.rst
--rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/docs/source/performance.rst
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/docs/source/typing.rst
--rw-r--r--   0        0        0     7739 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/docs/source/usage.rst
--rw-r--r--   0        0        0     5487 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/docs/source/examples/networkflow.md
--rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/docs/source/examples/portfolio.md
--rw-r--r--   0        0        0     7376 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/docs/source/examples/projects.md
--rw-r--r--   0        0        0     5216 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/docs/source/examples/regression.md
--rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/docs/source/examples/workforce.md
--rwxr-xr-x   0        0        0    41668 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/docs/source/examples/data/portfolio.csv
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/docs/source/examples/data/preferences.csv
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/docs/source/examples/data/projects.csv
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/docs/source/examples/data/shift_requirements.csv
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/docs/source/examples/data/teams.csv
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/src/gurobipy_pandas/__init__.py
--rw-r--r--   0        0        0    14121 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/src/gurobipy_pandas/accessors.py
--rw-r--r--   0        0        0     6951 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/src/gurobipy_pandas/api.py
--rw-r--r--   0        0        0     7202 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/src/gurobipy_pandas/constraints.py
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/src/gurobipy_pandas/index_mappers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/src/gurobipy_pandas/py.typed
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/src/gurobipy_pandas/util.py
--rw-r--r--   0        0        0     6054 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/src/gurobipy_pandas/variables.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0    26531 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/tests/test_accessors.py
--rw-r--r--   0        0        0    15736 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/tests/test_api.py
--rw-r--r--   0        0        0    19345 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/tests/test_constraints.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/tests/test_docs.py
--rw-r--r--   0        0        0     8758 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/tests/test_index_mappers.py
--rw-r--r--   0        0        0     9629 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/tests/test_operators.py
--rw-r--r--   0        0        0    24320 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/tests/test_variables.py
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/tests/utils.py
--rw-r--r--   0        0        0    15404 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/webinar/gppd-in-90-seconds.ipynb
--rw-r--r--   0        0        0   593807 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/webinar/gppd-in-90-seconds.slides.html
--rw-r--r--   0        0        0    90593 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/webinar/webinar.ipynb
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/.gitignore
--rw-r--r--   0        0        0    10976 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/LICENSE
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/README.md
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/.readthedocs.yaml
+-rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/Makefile
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/tox.ini
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/.github/workflows/build-wheel.yml
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/.github/workflows/code-quality.yml
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/.github/workflows/notebook-examples.yml
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/.github/workflows/publish-pypi.yml
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/.github/workflows/test-wheel.yml
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/.github/workflows/unit-tests.yml
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/docs/make.bat
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/docs/requirements-examples.txt
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/docs/requirements.txt
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/docs/source/acknowledgements.rst
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/docs/source/advanced.rst
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/docs/source/api.rst
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/docs/source/conf.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/docs/source/contact.rst
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/docs/source/examples.rst
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/docs/source/index.rst
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/docs/source/installation.rst
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/docs/source/license.rst
+-rw-r--r--   0        0        0     6209 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/docs/source/naming.rst
+-rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/docs/source/performance.rst
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/docs/source/typing.rst
+-rw-r--r--   0        0        0     7739 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/docs/source/usage.rst
+-rw-r--r--   0        0        0     7376 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/docs/source/examples/projects.md
+-rw-r--r--   0        0        0     5216 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/docs/source/examples/regression.md
+-rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/docs/source/examples/workforce.md
+-rwxr-xr-x   0        0        0    41668 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/docs/source/examples/data/portfolio.csv
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/docs/source/examples/data/preferences.csv
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/docs/source/examples/data/projects.csv
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/docs/source/examples/data/shift_requirements.csv
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/docs/source/examples/data/teams.csv
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/src/gurobipy_pandas/__init__.py
+-rw-r--r--   0        0        0    14121 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/src/gurobipy_pandas/accessors.py
+-rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/src/gurobipy_pandas/api.py
+-rw-r--r--   0        0        0     7202 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/src/gurobipy_pandas/constraints.py
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/src/gurobipy_pandas/index_mappers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/src/gurobipy_pandas/py.typed
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/src/gurobipy_pandas/util.py
+-rw-r--r--   0        0        0     6054 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/src/gurobipy_pandas/variables.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/tests/__init__.py
+-rw-r--r--   0        0        0    26531 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/tests/test_accessors.py
+-rw-r--r--   0        0        0    15736 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/tests/test_api.py
+-rw-r--r--   0        0        0    19345 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/tests/test_constraints.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/tests/test_docs.py
+-rw-r--r--   0        0        0     8758 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/tests/test_index_mappers.py
+-rw-r--r--   0        0        0     9629 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/tests/test_operators.py
+-rw-r--r--   0        0        0    24320 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/tests/test_variables.py
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/tests/utils.py
+-rw-r--r--   0        0        0    15404 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/webinar/gppd-in-90-seconds.ipynb
+-rw-r--r--   0        0        0   593807 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/webinar/gppd-in-90-seconds.slides.html
+-rw-r--r--   0        0        0    90593 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/webinar/webinar.ipynb
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/.gitignore
+-rw-r--r--   0        0        0    10976 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/LICENSE
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/README.md
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 gurobipy_pandas-1.1.2/PKG-INFO
```

### Comparing `gurobipy_pandas-1.1.1/CODE_OF_CONDUCT.md` & `gurobipy_pandas-1.1.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/CONTRIBUTING.md` & `gurobipy_pandas-1.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/Makefile` & `gurobipy_pandas-1.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/tox.ini` & `gurobipy_pandas-1.1.2/tox.ini`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/.github/workflows/build-wheel.yml` & `gurobipy_pandas-1.1.2/.github/workflows/build-wheel.yml`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 
 jobs:
   build-wheel:
 
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Setup Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.11"
       - name: Install build tools
         run: |
           python -m pip install --upgrade pip build
       - name: Build wheel and sdist
         run: |
```

### Comparing `gurobipy_pandas-1.1.1/.github/workflows/notebook-examples.yml` & `gurobipy_pandas-1.1.2/.github/workflows/notebook-examples.yml`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,17 @@
     strategy:
       matrix:
         os: [ubuntu-latest]
         python: ["3.8"]
         gurobipy: ["10.0.3", "11.0.0"]
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Setup Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python }}
       - name: Install tooling
         run: |
           python -m pip install --upgrade pip
       - name: Install dependencies
         run: |
```

### Comparing `gurobipy_pandas-1.1.1/.github/workflows/publish-pypi.yml` & `gurobipy_pandas-1.1.2/.github/workflows/publish-pypi.yml`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 on:
   workflow_call:
 
 jobs:
   publish-pypi:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Setup Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.11"
       - name: Install twine uploader
         run: |
           python -m pip install --upgrade pip
           python -m pip install twine
       - name: Fetch wheel artifact
```

### Comparing `gurobipy_pandas-1.1.1/.github/workflows/release.yml` & `gurobipy_pandas-1.1.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/.github/workflows/test-wheel.yml` & `gurobipy_pandas-1.1.2/.github/workflows/test-wheel.yml`

 * *Files 10% similar despite different names*

```diff
@@ -22,27 +22,29 @@
 
     runs-on: ${{ matrix.os }}
 
     strategy:
       matrix:
         os: [ubuntu-latest, windows-latest, macos-latest]
         python: ["3.8", "3.9", "3.10", "3.11", "3.12"]
-        gurobipy: ["10.0.3", "11.0.0"]
+        gurobipy: ["10.0.3", "11.0.2"]
         exclude:
           - python: "3.12"
             gurobipy: "10.0.3"
+          - os: macos-latest
+            python: "3.8"
 
     steps:
       - name: Checkout unit tests
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
         with:
           sparse-checkout: |
             tests
       - name: Setup Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python }}
       - name: File listing
         run: ls -R
       - name: Fetch built wheel
         uses: actions/download-artifact@v3
         with:
```

### Comparing `gurobipy_pandas-1.1.1/.github/workflows/unit-tests.yml` & `gurobipy_pandas-1.1.2/.github/workflows/unit-tests.yml`

 * *Files 14% similar despite different names*

```diff
@@ -12,21 +12,24 @@
   unit-tests:
 
     runs-on: ${{ matrix.os }}
 
     strategy:
       matrix:
         os: [ubuntu-latest]
-        python: ["3.8"]
-        gurobipy: ["10.0.3", "11.0.0"]
+        python: ["3.8", "3.12"]
+        gurobipy: ["10.0.3", "11.0.2"]
+        exclude:
+          - python: "3.12"
+            gurobipy: "10.0.3"
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Setup Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python }}
       - name: Install tooling
         run: |
           python -m pip install --upgrade pip
       - name: Install dependencies
         run: |
```

### Comparing `gurobipy_pandas-1.1.1/docs/Makefile` & `gurobipy_pandas-1.1.2/docs/Makefile`

 * *Files 8% similar despite different names*

```diff
@@ -13,11 +13,14 @@
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
 .PHONY: help watch Makefile
 
 livehtml:
 	sphinx-autobuild --open-browser "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
+cleannb:
+	rm -f source/examples/*.ipynb
+
 # Catch-all target: route all unknown targets to Sphinx using the new
 # "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
 %: Makefile
 	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `gurobipy_pandas-1.1.1/docs/make.bat` & `gurobipy_pandas-1.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/docs/source/advanced.rst` & `gurobipy_pandas-1.1.2/docs/source/advanced.rst`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/docs/source/conf.py` & `gurobipy_pandas-1.1.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/docs/source/examples.rst` & `gurobipy_pandas-1.1.2/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/docs/source/index.rst` & `gurobipy_pandas-1.1.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/docs/source/installation.rst` & `gurobipy_pandas-1.1.2/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/docs/source/license.rst` & `gurobipy_pandas-1.1.2/docs/source/license.rst`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/docs/source/naming.rst` & `gurobipy_pandas-1.1.2/docs/source/naming.rst`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/docs/source/performance.rst` & `gurobipy_pandas-1.1.2/docs/source/performance.rst`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/docs/source/typing.rst` & `gurobipy_pandas-1.1.2/docs/source/typing.rst`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/docs/source/usage.rst` & `gurobipy_pandas-1.1.2/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/docs/source/examples/projects.md` & `gurobipy_pandas-1.1.2/docs/source/examples/projects.md`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/docs/source/examples/regression.md` & `gurobipy_pandas-1.1.2/docs/source/examples/regression.md`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/docs/source/examples/workforce.md` & `gurobipy_pandas-1.1.2/docs/source/examples/workforce.md`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/docs/source/examples/data/portfolio.csv` & `gurobipy_pandas-1.1.2/docs/source/examples/data/portfolio.csv`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/docs/source/examples/data/preferences.csv` & `gurobipy_pandas-1.1.2/docs/source/examples/data/preferences.csv`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/src/gurobipy_pandas/accessors.py` & `gurobipy_pandas-1.1.2/src/gurobipy_pandas/accessors.py`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/src/gurobipy_pandas/api.py` & `gurobipy_pandas-1.1.2/src/gurobipy_pandas/api.py`

 * *Files 15% similar despite different names*

```diff
@@ -113,21 +113,40 @@
     Parameters
     ----------
     model : Model
         A Gurobi model to which new variables will be added
     pandas_obj : Index, Series, or DataFrame
         A pandas Index, Series, or DataFrame
     name : str, optional
-        If provided, used as base name for new Gurobi variables and the name
-        of the returned series
+        If provided, used as base name for new Gurobi variables and the name of
+        the returned series
     lb : float, str, or Series, optional
-        Lower bound for created variables. Can be a single numeric
-        value. If ``pandas_obj`` is an Index or Series, can be a Series
-        aligned with ``pandas_obj``. If ``pandas_obj`` is a dataframe,
-        can be a string referring to a column of ``pandas_obj``. Defaults to 0.0.
+        Lower bound for created variables. Can be a single numeric value. If
+        ``pandas_obj`` is an Index or Series, can be a Series aligned with
+        ``pandas_obj``. If ``pandas_obj`` is a dataframe, can be a string
+        referring to a column of ``pandas_obj``. Defaults to 0.0.
+    ub : float, str, or Series, optional
+        Upper bound for created variables. Can be a single numeric value. If
+        ``pandas_obj`` is an Index or Series, can be a Series aligned with
+        ``pandas_obj``. If ``pandas_obj`` is a dataframe, can be a string
+        referring to a column of ``pandas_obj``. Defaults to 0.0.
+    obj : float, str, or Series, optional
+        Linear objective function coefficient for created variables. Can be a
+        single numeric value. If ``pandas_obj`` is an Index or Series, can be a
+        Series aligned with ``pandas_obj``. If ``pandas_obj`` is a dataframe,
+        can be a string referring to a column of ``pandas_obj``. Defaults to
+        0.0.
+    vtype : str or Series, optional
+        Types of created variables. Can be a single string specifying the type
+        (e.g. ``GRB.BINARY``). If ``pandas_obj`` is an Index or Series, can be a
+        Series aligned with ``pandas_obj`` containing variable type string
+        values. Defaults to ``GRB.CONTINUOUS``.
+    index_formatter :
+        Can be used to provide custom conversion of index values to variable
+        names. The default behaviour is usually sufficient.
 
     Returns
     -------
     Series
         A Series of vars with the the index of `pandas_obj`
     """
     if isinstance(pandas_obj, pd.Index):
@@ -197,14 +216,17 @@
     rhs : Series or float
         A series of expressions forming the right hand side of constraints,
         or a common constant
     name : str
         Used as the returned series name, as well as the base name for added
         Gurobi constraints. Constraint name suffixes come from the lhs/rhs
         index.
+    index_formatter :
+        Can be used to provide custom conversion of index values to variable
+        names. The default behaviour is usually sufficient.
 
     Returns
     -------
     Series
            A Series of Constr objects
     """
     return add_constrs_from_series(
```

### Comparing `gurobipy_pandas-1.1.1/src/gurobipy_pandas/constraints.py` & `gurobipy_pandas-1.1.2/src/gurobipy_pandas/constraints.py`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/src/gurobipy_pandas/index_mappers.py` & `gurobipy_pandas-1.1.2/src/gurobipy_pandas/index_mappers.py`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/src/gurobipy_pandas/util.py` & `gurobipy_pandas-1.1.2/src/gurobipy_pandas/util.py`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/src/gurobipy_pandas/variables.py` & `gurobipy_pandas-1.1.2/src/gurobipy_pandas/variables.py`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/tests/test_accessors.py` & `gurobipy_pandas-1.1.2/tests/test_accessors.py`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/tests/test_api.py` & `gurobipy_pandas-1.1.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/tests/test_constraints.py` & `gurobipy_pandas-1.1.2/tests/test_constraints.py`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/tests/test_docs.py` & `gurobipy_pandas-1.1.2/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/tests/test_index_mappers.py` & `gurobipy_pandas-1.1.2/tests/test_index_mappers.py`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/tests/test_operators.py` & `gurobipy_pandas-1.1.2/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/tests/test_variables.py` & `gurobipy_pandas-1.1.2/tests/test_variables.py`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/tests/utils.py` & `gurobipy_pandas-1.1.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/webinar/gppd-in-90-seconds.ipynb` & `gurobipy_pandas-1.1.2/webinar/gppd-in-90-seconds.ipynb`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/webinar/gppd-in-90-seconds.slides.html` & `gurobipy_pandas-1.1.2/webinar/gppd-in-90-seconds.slides.html`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/webinar/webinar.ipynb` & `gurobipy_pandas-1.1.2/webinar/webinar.ipynb`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/.gitignore` & `gurobipy_pandas-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/LICENSE` & `gurobipy_pandas-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/README.md` & `gurobipy_pandas-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/pyproject.toml` & `gurobipy_pandas-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gurobipy_pandas-1.1.1/PKG-INFO` & `gurobipy_pandas-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: gurobipy-pandas
-Version: 1.1.1
+Version: 1.1.2
 Summary: Pandas accessors for gurobipy interaction
 Project-URL: Documentation, https://gurobi-optimization-gurobipy-pandas.readthedocs-hosted.com/en/latest
 Project-URL: Issues, https://github.com/Gurobi/gurobipy-pandas/issues
 Project-URL: Source, https://github.com/Gurobi/gurobipy-pandas
 Author-email: Simon Bowly <bowly@gurobi.com>, Robert Luce <luce@gurobi.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

