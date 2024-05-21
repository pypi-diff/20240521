# Comparing `tmp/pydicomsorter-0.4.0.tar.gz` & `tmp/pydicomsorter-0.4.1.tar.gz`

## Comparing `pydicomsorter-0.4.0.tar` & `pydicomsorter-0.4.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/.pypackage-builder-answers.yml
--rw-r--r--   0        0        0   221972 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/pixi.lock
--rw-r--r--   0        0        0     9532 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/.github/workflows/main.yaml
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/config/coverage.toml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/config/hatch.toml
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/config/mkdocs.yaml
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/config/releaserc.toml
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/config/ruff.toml
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/docs/CHANGELOG.md
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/docs/about.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/docs/index.md
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/src/pydicomsorter/__init__.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/src/pydicomsorter/io.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/src/pydicomsorter/main.py
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/src/pydicomsorter/parser.py
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/src/pydicomsorter/tags4format.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/src/pydicomsorter/sandbox/__init__.py
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/src/pydicomsorter/sandbox/diffwork.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/tests/test_parser.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/tests/test_say_hello.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/LICENSE
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/README.md
--rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pydicomsorter-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/.pypackage-builder-answers.yml
+-rw-r--r--   0        0        0   221972 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/pixi.lock
+-rw-r--r--   0        0        0     9497 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/.github/workflows/main.yaml
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/config/coverage.toml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/config/hatch.toml
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/config/mkdocs.yaml
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/config/releaserc.toml
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/config/ruff.toml
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/docs/about.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/docs/index.md
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/src/pydicomsorter/__init__.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/src/pydicomsorter/io.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/src/pydicomsorter/main.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/src/pydicomsorter/parser.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/src/pydicomsorter/tags4format.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/src/pydicomsorter/sandbox/__init__.py
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/src/pydicomsorter/sandbox/diffwork.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/tests/test_parser.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/tests/test_say_hello.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/LICENSE
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/README.md
+-rw-r--r--   0        0        0     4741 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pydicomsorter-0.4.1/PKG-INFO
```

### Comparing `pydicomsorter-0.4.0/pixi.lock` & `pydicomsorter-0.4.1/pixi.lock`

 * *Files 1% similar despite different names*

```diff
@@ -3900,17 +3900,17 @@
   - sphinx-rtd-theme ; extra == 'docs'
   - sphinx-gallery ; extra == 'docs'
   - sphinxcontrib-napoleon ; extra == 'docs'
   - sphinx-copybutton ; extra == 'docs'
   requires_python: '>=3.7'
 - kind: pypi
   name: pydicomsorter
-  version: 0.4.0
+  version: 0.4.1
   path: .
-  sha256: 1e0cac8e9f0e675b7662a19ba328e238d61d364d337cc8d7b6138e5c87f53980
+  sha256: 64335c4f4dbf9c666e3326d8854eb46d8e0740cf9931b6db34349a52cc4e1077
   requires_dist:
   - rich
   - rich-click
   - pydicom
   requires_python: '>=3.12'
   editable: true
 - kind: pypi
```

### Comparing `pydicomsorter-0.4.0/.github/workflows/main.yaml` & `pydicomsorter-0.4.1/.github/workflows/main.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
       - name: Run pytest
         run: |
           pixi run which python
           pixi run test
 
       - name: Upload coverage report artifact to be used by Codecov
         # only upload if matrix.os is ubuntu-latest and matrix.python-version is 3.12
-        if: matrix.os == 'ubuntu-latest' && matrix.python-version == '3.12'
+        if: matrix.os == 'ubuntu-latest'
         uses: actions/upload-artifact@v2
         with:
           name: coverage-report
           path: coverage-report
 
   ################################################################################################
   # Codecov: Run codecov to check coverage
```

### Comparing `pydicomsorter-0.4.0/config/mkdocs.yaml` & `pydicomsorter-0.4.1/config/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.4.0/config/releaserc.toml` & `pydicomsorter-0.4.1/config/releaserc.toml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.4.0/config/ruff.toml` & `pydicomsorter-0.4.1/config/ruff.toml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.4.0/docs/CHANGELOG.md` & `pydicomsorter-0.4.1/docs/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 # CHANGELOG
 
 
 
+## v0.4.1 (2024-05-21)
+
+### Fix
+
+* fix: lock ([`9711580`](https://github.com/jjjermiah/PyDicomSorter/commit/9711580d2decb816113b45d0cb44b4b74c26d8d7))
+
+* fix: enforce code upload ([`ba93172`](https://github.com/jjjermiah/PyDicomSorter/commit/ba93172023f9c56eaac91b5f95270d0330e33d4b))
+
+
 ## v0.4.0 (2024-05-21)
 
 ### Feature
 
 * feat: add codecov badge and fix lock ([`00986a8`](https://github.com/jjjermiah/PyDicomSorter/commit/00986a81e0f24c5d67c7c72a29d04888151b2317))
 
 * feat: upload to codecov ([`97ac6bb`](https://github.com/jjjermiah/PyDicomSorter/commit/97ac6bbf1b241ed8afd331188f8d3624cbe087dc))
```

### Comparing `pydicomsorter-0.4.0/docs/about.md` & `pydicomsorter-0.4.1/docs/about.md`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.4.0/src/pydicomsorter/parser.py` & `pydicomsorter-0.4.1/src/pydicomsorter/parser.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.4.0/src/pydicomsorter/tags4format.py` & `pydicomsorter-0.4.1/src/pydicomsorter/tags4format.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.4.0/src/pydicomsorter/sandbox/diffwork.py` & `pydicomsorter-0.4.1/src/pydicomsorter/sandbox/diffwork.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.4.0/tests/test_parser.py` & `pydicomsorter-0.4.1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.4.0/.gitignore` & `pydicomsorter-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.4.0/LICENSE` & `pydicomsorter-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.4.0/pyproject.toml` & `pydicomsorter-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #--------------------------------------------------------------------------------------------------#
 ######################################### Package Config ###########################################
 #__________________________________________________________________________________________________#
 [project]
 name = "pydicomsorter"
-version = "0.4.0"
+version = "0.4.1"
 description = "A Quick Tool For Sorting Dicom Files"
 license = "MIT"
 readme = "README.md"
 keywords = ["pydicomsorter", "pixi", "python", "package"]
 
 authors = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
 maintainers = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
```

### Comparing `pydicomsorter-0.4.0/PKG-INFO` & `pydicomsorter-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pydicomsorter
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Quick Tool For Sorting Dicom Files
 Project-URL: homepage, https://github.com/jjjermiah/pydicomsorter
 Project-URL: repository, https://github.com/jjjermiah/pydicomsorter
 Project-URL: documentation, https://jjjermiah.github.io/pydicomsorter/
 Project-URL: changelog, https://github.com/jjjermiah/pydicomsorter/blob/main/docs/CHANGELOG.md
 Project-URL: issues, https://github.com/jjjermiah/pydicomsorter/issues
 Author-email: Jermiah Joseph <jermiahjoseph98@gmail.com>
```

