# Comparing `tmp/pydicomsorter-0.3.0.tar.gz` & `tmp/pydicomsorter-0.4.0.tar.gz`

## Comparing `pydicomsorter-0.3.0.tar` & `pydicomsorter-0.4.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pydicomsorter-0.3.0/.pypackage-builder-answers.yml
--rw-r--r--   0        0        0   221972 2020-02-02 00:00:00.000000 pydicomsorter-0.3.0/pixi.lock
--rw-r--r--   0        0        0     8701 2020-02-02 00:00:00.000000 pydicomsorter-0.3.0/.github/workflows/main.yaml
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pydicomsorter-0.3.0/config/coverage.toml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydicomsorter-0.3.0/config/hatch.toml
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 pydicomsorter-0.3.0/config/mkdocs.yaml
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 pydicomsorter-0.3.0/config/releaserc.toml
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pydicomsorter-0.3.0/config/ruff.toml
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 pydicomsorter-0.3.0/docs/CHANGELOG.md
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 pydicomsorter-0.3.0/docs/about.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pydicomsorter-0.3.0/docs/index.md
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 pydicomsorter-0.3.0/src/pydicomsorter/__init__.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 pydicomsorter-0.3.0/src/pydicomsorter/io.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 pydicomsorter-0.3.0/src/pydicomsorter/main.py
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pydicomsorter-0.3.0/src/pydicomsorter/parser.py
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 pydicomsorter-0.3.0/src/pydicomsorter/tags4format.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pydicomsorter-0.3.0/src/pydicomsorter/sandbox/__init__.py
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 pydicomsorter-0.3.0/src/pydicomsorter/sandbox/diffwork.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 pydicomsorter-0.3.0/tests/test_parser.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pydicomsorter-0.3.0/tests/test_say_hello.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 pydicomsorter-0.3.0/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 pydicomsorter-0.3.0/LICENSE
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 pydicomsorter-0.3.0/README.md
--rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 pydicomsorter-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 pydicomsorter-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/.pypackage-builder-answers.yml
+-rw-r--r--   0        0        0   221972 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/pixi.lock
+-rw-r--r--   0        0        0     9532 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/.github/workflows/main.yaml
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/config/coverage.toml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/config/hatch.toml
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/config/mkdocs.yaml
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/config/releaserc.toml
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/config/ruff.toml
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/docs/about.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/docs/index.md
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/src/pydicomsorter/__init__.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/src/pydicomsorter/io.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/src/pydicomsorter/main.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/src/pydicomsorter/parser.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/src/pydicomsorter/tags4format.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/src/pydicomsorter/sandbox/__init__.py
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/src/pydicomsorter/sandbox/diffwork.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/tests/test_parser.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/tests/test_say_hello.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/LICENSE
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/README.md
+-rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/PKG-INFO
```

### Comparing `pydicomsorter-0.3.0/pixi.lock` & `pydicomsorter-0.4.0/pixi.lock`

 * *Files 0% similar despite different names*

```diff
@@ -3900,17 +3900,17 @@
   - sphinx-rtd-theme ; extra == 'docs'
   - sphinx-gallery ; extra == 'docs'
   - sphinxcontrib-napoleon ; extra == 'docs'
   - sphinx-copybutton ; extra == 'docs'
   requires_python: '>=3.7'
 - kind: pypi
   name: pydicomsorter
-  version: 0.3.0
+  version: 0.4.0
   path: .
-  sha256: 79a4477e5f9ca0617bb3bff4898abc664e1333f3802ff8e28b47e5cab590d191
+  sha256: 1e0cac8e9f0e675b7662a19ba328e238d61d364d337cc8d7b6138e5c87f53980
   requires_dist:
   - rich
   - rich-click
   - pydicom
   requires_python: '>=3.12'
   editable: true
 - kind: pypi
```

### Comparing `pydicomsorter-0.3.0/.github/workflows/main.yaml` & `pydicomsorter-0.4.0/.github/workflows/main.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,39 @@
         if: matrix.os == 'ubuntu-latest' && matrix.python-version == '3.12'
         uses: actions/upload-artifact@v2
         with:
           name: coverage-report
           path: coverage-report
 
   ################################################################################################
+  # Codecov: Run codecov to check coverage
+  ################################################################################################
+  Code-Coverage:
+    needs: Unit-Tests
+    runs-on: ubuntu-latest
+    steps:
+      - name: Checkout code
+        uses: actions/checkout@v3
+
+      - name: Download coverage.xml artifact
+        uses: actions/download-artifact@v2
+        with:
+          name: coverage-report
+          path: coverage-report
+
+      - name: Use Codecov to track coverage
+        uses: codecov/codecov-action@v3
+        with:
+          token: ${{ secrets.CODECOV_TOKEN }}
+          files: ./coverage-report/coverage.xml
+          fail_ci_if_error: true
+          verbose: true
+          name: codecov-umbrella
+
+  ################################################################################################
   # Ruff: Run ruff linter
   ################################################################################################
   Ruff:
     runs-on: ubuntu-latest
     env:
       PIXI_ENV: "dev"
     strategy:
```

### Comparing `pydicomsorter-0.3.0/config/mkdocs.yaml` & `pydicomsorter-0.4.0/config/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.3.0/config/releaserc.toml` & `pydicomsorter-0.4.0/config/releaserc.toml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.3.0/config/ruff.toml` & `pydicomsorter-0.4.0/config/ruff.toml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.3.0/docs/CHANGELOG.md` & `pydicomsorter-0.4.0/docs/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 # CHANGELOG
 
 
 
+## v0.4.0 (2024-05-21)
+
+### Feature
+
+* feat: add codecov badge and fix lock ([`00986a8`](https://github.com/jjjermiah/PyDicomSorter/commit/00986a81e0f24c5d67c7c72a29d04888151b2317))
+
+* feat: upload to codecov ([`97ac6bb`](https://github.com/jjjermiah/PyDicomSorter/commit/97ac6bbf1b241ed8afd331188f8d3624cbe087dc))
+
+
 ## v0.3.0 (2024-05-21)
 
 ### Feature
 
 * feat: move mkdocs config to a config directory ([`7a7cf35`](https://github.com/jjjermiah/PyDicomSorter/commit/7a7cf35561974c3985dfcadf69568c451539bd5f))
 
 ### Fix
```

### Comparing `pydicomsorter-0.3.0/docs/about.md` & `pydicomsorter-0.4.0/docs/about.md`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.3.0/src/pydicomsorter/parser.py` & `pydicomsorter-0.4.0/src/pydicomsorter/parser.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.3.0/src/pydicomsorter/tags4format.py` & `pydicomsorter-0.4.0/src/pydicomsorter/tags4format.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.3.0/src/pydicomsorter/sandbox/diffwork.py` & `pydicomsorter-0.4.0/src/pydicomsorter/sandbox/diffwork.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.3.0/tests/test_parser.py` & `pydicomsorter-0.4.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.3.0/.gitignore` & `pydicomsorter-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.3.0/LICENSE` & `pydicomsorter-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.3.0/pyproject.toml` & `pydicomsorter-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #--------------------------------------------------------------------------------------------------#
 ######################################### Package Config ###########################################
 #__________________________________________________________________________________________________#
 [project]
 name = "pydicomsorter"
-version = "0.3.0"
+version = "0.4.0"
 description = "A Quick Tool For Sorting Dicom Files"
 license = "MIT"
 readme = "README.md"
 keywords = ["pydicomsorter", "pixi", "python", "package"]
 
 authors = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
 maintainers = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
```

### Comparing `pydicomsorter-0.3.0/PKG-INFO` & `pydicomsorter-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pydicomsorter
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Quick Tool For Sorting Dicom Files
 Project-URL: homepage, https://github.com/jjjermiah/pydicomsorter
 Project-URL: repository, https://github.com/jjjermiah/pydicomsorter
 Project-URL: documentation, https://jjjermiah.github.io/pydicomsorter/
 Project-URL: changelog, https://github.com/jjjermiah/pydicomsorter/blob/main/docs/CHANGELOG.md
 Project-URL: issues, https://github.com/jjjermiah/pydicomsorter/issues
 Author-email: Jermiah Joseph <jermiahjoseph98@gmail.com>
@@ -17,9 +17,10 @@
 Requires-Dist: rich
 Requires-Dist: rich-click
 Description-Content-Type: text/markdown
 
 # pydicomsorter
 
 =============================
+[![codecov](https://codecov.io/gh/jjjermiah/PyDicomSorter/graph/badge.svg?token=tCcajRIGz9)](https://codecov.io/gh/jjjermiah/PyDicomSorter)
 
 Testing the pydicom library to sort dicom files by patient name and study date.
```

