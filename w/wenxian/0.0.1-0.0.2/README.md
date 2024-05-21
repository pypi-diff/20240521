# Comparing `tmp/wenxian-0.0.1.tar.gz` & `tmp/wenxian-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wenxian-0.0.1.tar", last modified: Mon May 20 06:11:19 2024, max compression
+gzip compressed data, was "wenxian-0.0.2.tar", last modified: Tue May 21 08:11:15 2024, max compression
```

## Comparing `wenxian-0.0.1.tar` & `wenxian-0.0.2.tar`

### file list

```diff
@@ -1,43 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:11:19.963055 wenxian-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-20 06:11:15.000000 wenxian-0.0.1/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-20 06:11:15.000000 wenxian-0.0.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:11:19.955056 wenxian-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:11:19.955056 wenxian-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-20 06:11:15.000000 wenxian-0.0.1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-20 06:11:15.000000 wenxian-0.0.1/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-05-20 06:11:15.000000 wenxian-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-20 06:11:15.000000 wenxian-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-20 06:11:15.000000 wenxian-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10726 2024-05-20 06:11:19.963055 wenxian-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-20 06:11:15.000000 wenxian-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-20 06:11:15.000000 wenxian-0.0.1/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-20 06:11:15.000000 wenxian-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 06:11:19.963055 wenxian-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:11:19.959056 wenxian-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-20 06:11:15.000000 wenxian-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19887 2024-05-20 06:11:15.000000 wenxian-0.0.1/tests/cases.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-20 06:11:15.000000 wenxian-0.0.1/tests/test_bibtex.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-20 06:11:15.000000 wenxian-0.0.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-20 06:11:15.000000 wenxian-0.0.1/tests/test_from_identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-20 06:11:15.000000 wenxian-0.0.1/tests/test_identifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:11:19.959056 wenxian-0.0.1/wenxian/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-20 06:11:16.000000 wenxian-0.0.1/wenxian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-20 06:11:16.000000 wenxian-0.0.1/wenxian/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:11:19.963055 wenxian-0.0.1/wenxian/feeder/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-20 06:11:16.000000 wenxian-0.0.1/wenxian/feeder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-20 06:11:16.000000 wenxian-0.0.1/wenxian/feeder/arxiv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-20 06:11:16.000000 wenxian-0.0.1/wenxian/feeder/crossref.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-20 06:11:16.000000 wenxian-0.0.1/wenxian/feeder/feeder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-05-20 06:11:16.000000 wenxian-0.0.1/wenxian/feeder/pubmed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-20 06:11:16.000000 wenxian-0.0.1/wenxian/feeder/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-20 06:11:16.000000 wenxian-0.0.1/wenxian/from_identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-20 06:11:16.000000 wenxian-0.0.1/wenxian/identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 06:11:16.000000 wenxian-0.0.1/wenxian/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-05-20 06:11:16.000000 wenxian-0.0.1/wenxian/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:11:19.963055 wenxian-0.0.1/wenxian.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10726 2024-05-20 06:11:19.000000 wenxian-0.0.1/wenxian.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-20 06:11:19.000000 wenxian-0.0.1/wenxian.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 06:11:19.000000 wenxian-0.0.1/wenxian.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-20 06:11:19.000000 wenxian-0.0.1/wenxian.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-20 06:11:19.000000 wenxian-0.0.1/wenxian.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-20 06:11:19.000000 wenxian-0.0.1/wenxian.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:11:15.444022 wenxian-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-21 08:11:11.000000 wenxian-0.0.2/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 08:11:11.000000 wenxian-0.0.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:11:15.436022 wenxian-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:11:15.440022 wenxian-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-21 08:11:11.000000 wenxian-0.0.2/.github/workflows/comment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-21 08:11:11.000000 wenxian-0.0.2/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-21 08:11:11.000000 wenxian-0.0.2/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-21 08:11:11.000000 wenxian-0.0.2/.github/workflows/test_action.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-05-21 08:11:11.000000 wenxian-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-21 08:11:11.000000 wenxian-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-21 08:11:11.000000 wenxian-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11855 2024-05-21 08:11:15.444022 wenxian-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-21 08:11:11.000000 wenxian-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-21 08:11:11.000000 wenxian-0.0.2/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:11:15.440022 wenxian-0.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 08:11:11.000000 wenxian-0.0.2/docs/CNAME
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-05-21 08:11:11.000000 wenxian-0.0.2/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-05-21 08:11:11.000000 wenxian-0.0.2/docs/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-21 08:11:11.000000 wenxian-0.0.2/docs/pyworker.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-21 08:11:11.000000 wenxian-0.0.2/docs/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-21 08:11:11.000000 wenxian-0.0.2/docs/webworker.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-21 08:11:11.000000 wenxian-0.0.2/docs/wenxian.js
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-21 08:11:11.000000 wenxian-0.0.2/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-21 08:11:11.000000 wenxian-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 08:11:15.444022 wenxian-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:11:15.440022 wenxian-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 08:11:11.000000 wenxian-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21737 2024-05-21 08:11:11.000000 wenxian-0.0.2/tests/cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-21 08:11:11.000000 wenxian-0.0.2/tests/test_bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-21 08:11:11.000000 wenxian-0.0.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-21 08:11:11.000000 wenxian-0.0.2/tests/test_from_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-21 08:11:11.000000 wenxian-0.0.2/tests/test_identifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:11:15.444022 wenxian-0.0.2/wenxian/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-21 08:11:11.000000 wenxian-0.0.2/wenxian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-21 08:11:11.000000 wenxian-0.0.2/wenxian/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:11:15.444022 wenxian-0.0.2/wenxian/feeder/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-21 08:11:11.000000 wenxian-0.0.2/wenxian/feeder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-21 08:11:11.000000 wenxian-0.0.2/wenxian/feeder/arxiv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-21 08:11:11.000000 wenxian-0.0.2/wenxian/feeder/crossref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-21 08:11:11.000000 wenxian-0.0.2/wenxian/feeder/feeder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-05-21 08:11:11.000000 wenxian-0.0.2/wenxian/feeder/pubmed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-21 08:11:11.000000 wenxian-0.0.2/wenxian/feeder/semanticscholar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-21 08:11:11.000000 wenxian-0.0.2/wenxian/feeder/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-21 08:11:11.000000 wenxian-0.0.2/wenxian/from_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-21 08:11:11.000000 wenxian-0.0.2/wenxian/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:11:11.000000 wenxian-0.0.2/wenxian/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-05-21 08:11:11.000000 wenxian-0.0.2/wenxian/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:11:15.444022 wenxian-0.0.2/wenxian.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11855 2024-05-21 08:11:15.000000 wenxian-0.0.2/wenxian.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-21 08:11:15.000000 wenxian-0.0.2/wenxian.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 08:11:15.000000 wenxian-0.0.2/wenxian.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-21 08:11:15.000000 wenxian-0.0.2/wenxian.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-21 08:11:15.000000 wenxian-0.0.2/wenxian.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-21 08:11:15.000000 wenxian-0.0.2/wenxian.egg-info/top_level.txt
```

### Comparing `wenxian-0.0.1/.github/workflows/release.yaml` & `wenxian-0.0.2/.github/workflows/release.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 on:
   push:
     branches:
       - master
     tags:
-      - 'v*'
+      - "v*"
   pull_request:
 name: Build and release to pypi
 jobs:
   release-build:
     name: Build and upload distributions
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v4
-    - name: Setup python
-      uses: actions/setup-python@v5
-      with:
-        python-version: 3.x
-    - run: pipx run build
-    - name: Upload release distributions
-      uses: actions/upload-artifact@v4
-      with:
-        name: release-dists
-        path: dist/
+      - uses: actions/checkout@v4
+      - name: Setup python
+        uses: actions/setup-python@v5
+        with:
+          python-version: 3.x
+      - run: pipx run build
+      - name: Upload release distributions
+        uses: actions/upload-artifact@v4
+        with:
+          name: release-dists
+          path: dist/
   pypi-publish:
     name: Release to pypi
     runs-on: ubuntu-latest
     environment:
       name: pypi_publish
       url: https://pypi.org/p/wenxian
     if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags/v')
```

### Comparing `wenxian-0.0.1/.github/workflows/test.yaml` & `wenxian-0.0.2/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.1/.gitignore` & `wenxian-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.1/LICENSE` & `wenxian-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.1/pyproject.toml` & `wenxian-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.1/tests/cases.py` & `wenxian-0.0.2/tests/cases.py`

 * *Files 4% similar despite different names*

```diff
@@ -334,8 +334,47 @@
                          current major version of the DeePMD-kit package, highlighting its
                          features and technical details. Additionally, this article presents a
                          comprehensive procedure for conducting molecular dynamics as a
                          representative application, benchmarks the accuracy and efficiency of
                          different models, and discusses ongoing developments.},
             }""").strip(),
     ),
+    # semanticscholar abstract
+    ReferenceCase(
+        reference=Reference(
+            author=[
+                Author(first="Jinzhe", last="Zeng"),
+                Author(first="Linfeng", last="Zhang"),
+                Author(first="Han", last="Wang"),
+                Author(first="Tong", last="Zhu"),
+            ],
+            title="Exploring the Chemical Space of Linear Alkane Pyrolysis via Deep Potential GENerator",
+            journal="Energy Fuels",
+            year=2021,
+            volume=35,
+            issue=1,
+            pages=(762, 769),
+            annote=textwrap.dedent("""\
+                Reactive molecular dynamics (MD) simulation is a powerful tool to study the reaction
+                mechanism of complex chemical systems. Central to the method is the potential energy
+                surface (PES) that can desc...""")
+            .strip()
+            .replace("\n", " "),
+            doi="10.1021/acs.energyfuels.0c03211",
+        ),
+        expected_bibtex=textwrap.dedent(r"""
+            @Article{Zeng_EnergyFuels_2021_v35_p762,
+                author =   {Jinzhe Zeng and Linfeng Zhang and Han Wang and Tong Zhu},
+                title =    {{Exploring the Chemical Space of Linear Alkane Pyrolysis via Deep
+                         Potential GENerator}},
+                journal =  {Energy Fuels},
+                year =     2021,
+                volume =   35,
+                issue =    1,
+                pages =    {762--769},
+                doi =      {10.1021/acs.energyfuels.0c03211},
+                annote =   {Reactive molecular dynamics (MD) simulation is a powerful tool to
+                         study the reaction mechanism of complex chemical systems. Central to
+                         the method is the potential energy surface (PES) that can desc...},
+            }""").strip(),
+    ),
 ]
```

### Comparing `wenxian-0.0.1/tests/test_cli.py` & `wenxian-0.0.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.1/tests/test_from_identifier.py` & `wenxian-0.0.2/tests/test_from_identifier.py`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.1/wenxian/__main__.py` & `wenxian-0.0.2/wenxian/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     output: str | None = None,
     **kwargs,
 ):
     """Generate BibTeX from a identifier."""
     buff = []
     references = []
     for identifier in IDENTIFIER:
-        ref = from_identifier(identifier)
+        ref = from_identifier(identifier.strip())
         if ref is None or ref.is_empty():
             raise ValueError(f"Failed to fetch reference from {identifier}")
         references.append(ref)
         buff.append(ref.bibtex)
     if output is None:
         sys.stdout.write("\n".join(buff))
         return
```

### Comparing `wenxian-0.0.1/wenxian/feeder/arxiv.py` & `wenxian-0.0.2/wenxian/feeder/arxiv.py`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.1/wenxian/feeder/crossref.py` & `wenxian-0.0.2/wenxian/feeder/crossref.py`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.1/wenxian/feeder/feeder.py` & `wenxian-0.0.2/wenxian/feeder/feeder.py`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.1/wenxian/feeder/pubmed.py` & `wenxian-0.0.2/wenxian/feeder/pubmed.py`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.1/wenxian/feeder/session.py` & `wenxian-0.0.2/wenxian/feeder/session.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,11 +31,14 @@
 adapter_crossref = LimiterAdapter(per_second=50, max_retries=retries)
 SESSION.mount("https://api.crossref.org/", adapter_crossref)
 # Arxiv: https://info.arxiv.org/help/api/tou.html
 adapter_arxiv = LimiterAdapter(
     limiter=Limiter(RequestRate(1, Duration.SECOND * 3)), burst=1, max_retries=retries
 )
 SESSION.mount("https://export.arxiv.org/api", adapter_arxiv)
+# https://www.semanticscholar.org/product/api
+adapter_semanticscholar = LimiterAdapter(per_second=1, max_retries=retries)
+SESSION.mount("https://api.semanticscholar.org/", adapter_semanticscholar)
 
 SESSION.mount("https://", HTTPAdapter(max_retries=retries))
 
 __all__ = ["SESSION"]
```

### Comparing `wenxian-0.0.1/wenxian/from_identifier.py` & `wenxian-0.0.2/wenxian/from_identifier.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 """Fetch a reference from an identifier."""
 
 from __future__ import annotations
 
 from wenxian.feeder.arxiv import Arxiv
 from wenxian.feeder.crossref import Crossref
 from wenxian.feeder.pubmed import Pubmed
+from wenxian.feeder.semanticscholar import Semanticscholar
 from wenxian.identifier import Identifier, get_identifier_type
 from wenxian.reference import Reference
 
 
 def from_doi(doi: str) -> Reference | None:
     """Fetch a reference from a DOI."""
     # pubmed is the most reliable source
     return (
         Reference()
         | Pubmed().from_doi(doi)
         | Crossref().from_doi(doi)
         | Arxiv().from_doi(doi)
+        | Semanticscholar().from_doi(doi)
     )
 
 
 def from_pmid(pmid: str | int) -> Reference | None:
     """Fetch a reference from a PMID."""
     # no need to fetch from crossref - pubmed usually has all information
     return Reference() | Pubmed().from_pmid(pmid)
 
 
 def from_arxiv(arxiv: str) -> Reference | None:
     """Fetch a reference from an arXiv identifier."""
+    # arxiv api has all information for arxiv papers
     return Reference() | Arxiv().from_arxiv(arxiv)
 
 
 def from_identifier(identifier: str) -> Reference | None:
     """Fetch a reference from an identifier."""
     identifier_type = get_identifier_type(identifier)
     if identifier_type is None:
```

### Comparing `wenxian-0.0.1/wenxian/identifier.py` & `wenxian-0.0.2/wenxian/identifier.py`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.1/wenxian/reference.py` & `wenxian-0.0.2/wenxian/reference.py`

 * *Files identical despite different names*

### Comparing `wenxian-0.0.1/wenxian.egg-info/SOURCES.txt` & `wenxian-0.0.2/wenxian.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 .git_archival.txt
 .gitattributes
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 README.md
+action.yml
 noxfile.py
 pyproject.toml
+.github/workflows/comment.yaml
 .github/workflows/release.yaml
 .github/workflows/test.yaml
+.github/workflows/test_action.yaml
+docs/CNAME
+docs/index.html
+docs/logo.svg
+docs/pyworker.js
+docs/style.css
+docs/webworker.js
+docs/wenxian.js
 tests/__init__.py
 tests/cases.py
 tests/test_bibtex.py
 tests/test_cli.py
 tests/test_from_identifier.py
 tests/test_identifier.py
 wenxian/__init__.py
@@ -27,8 +37,9 @@
 wenxian.egg-info/requires.txt
 wenxian.egg-info/top_level.txt
 wenxian/feeder/__init__.py
 wenxian/feeder/arxiv.py
 wenxian/feeder/crossref.py
 wenxian/feeder/feeder.py
 wenxian/feeder/pubmed.py
+wenxian/feeder/semanticscholar.py
 wenxian/feeder/session.py
```

