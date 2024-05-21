# Comparing `tmp/dom_tokenizers-0.0.7.tar.gz` & `tmp/dom_tokenizers-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dom_tokenizers-0.0.7.tar", last modified: Sun May 19 14:33:44 2024, max compression
+gzip compressed data, was "dom_tokenizers-0.0.8.tar", last modified: Mon May 20 00:19:28 2024, max compression
```

## Comparing `dom_tokenizers-0.0.7.tar` & `dom_tokenizers-0.0.8.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:33:44.354430 dom_tokenizers-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-19 14:33:44.354430 dom_tokenizers-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 14:33:44.354430 dom_tokenizers-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:33:44.350429 dom_tokenizers-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:33:44.350429 dom_tokenizers-0.0.7/src/dom_tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/src/dom_tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/src/dom_tokenizers/dump.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:33:44.354430 dom_tokenizers-0.0.7/src/dom_tokenizers/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/src/dom_tokenizers/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/src/dom_tokenizers/internal/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:33:44.354430 dom_tokenizers-0.0.7/src/dom_tokenizers/pre_tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/src/dom_tokenizers/pre_tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9570 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/src/dom_tokenizers/pre_tokenizers/dom_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/src/dom_tokenizers/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:33:44.354430 dom_tokenizers-0.0.7/src/dom_tokenizers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-19 14:33:44.000000 dom_tokenizers-0.0.7/src/dom_tokenizers.egg-info/SOURCES.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:33:44.354430 dom_tokenizers-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:33:44.354430 dom_tokenizers-0.0.7/tests/pre_tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/tests/pre_tokenizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:33:44.354430 dom_tokenizers-0.0.7/tests/pre_tokenizers/dom_snapshot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/tests/pre_tokenizers/dom_snapshot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/tests/pre_tokenizers/dom_snapshot/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/tests/pre_tokenizers/dom_snapshot/test_pre_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:33:44.354430 dom_tokenizers-0.0.7/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/tests/resources/raw-browser-response.html
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/tests/resources/raw-browser-response.json
--rw-r--r--   0 runner    (1001) docker     (127)    47499 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/tests/resources/svg-in-base64.html
--rw-r--r--   0 runner    (1001) docker     (127)    48905 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/tests/resources/svg-in-base64.json
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/tests/test_train_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-19 14:33:02.000000 dom_tokenizers-0.0.7/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:19:28.473863 dom_tokenizers-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-20 00:19:28.473863 dom_tokenizers-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 00:19:28.473863 dom_tokenizers-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:19:28.465863 dom_tokenizers-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:19:28.469863 dom_tokenizers-0.0.8/src/dom_tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/src/dom_tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/src/dom_tokenizers/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/src/dom_tokenizers/dump.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:19:28.469863 dom_tokenizers-0.0.8/src/dom_tokenizers/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/src/dom_tokenizers/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/src/dom_tokenizers/internal/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:19:28.469863 dom_tokenizers-0.0.8/src/dom_tokenizers/pre_tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/src/dom_tokenizers/pre_tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9570 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/src/dom_tokenizers/pre_tokenizers/dom_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/src/dom_tokenizers/tokenizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/src/dom_tokenizers/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:19:28.473863 dom_tokenizers-0.0.8/src/dom_tokenizers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-20 00:19:28.000000 dom_tokenizers-0.0.8/src/dom_tokenizers.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:19:28.469863 dom_tokenizers-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:19:28.469863 dom_tokenizers-0.0.8/tests/pre_tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/tests/pre_tokenizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:19:28.469863 dom_tokenizers-0.0.8/tests/pre_tokenizers/dom_snapshot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/tests/pre_tokenizers/dom_snapshot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/tests/pre_tokenizers/dom_snapshot/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/tests/pre_tokenizers/dom_snapshot/test_pre_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:19:28.473863 dom_tokenizers-0.0.8/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/tests/resources/raw-browser-response.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/tests/resources/raw-browser-response.json
+-rw-r--r--   0 runner    (1001) docker     (127)    47499 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/tests/resources/svg-in-base64.html
+-rw-r--r--   0 runner    (1001) docker     (127)    48905 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/tests/resources/svg-in-base64.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/tests/test_train_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-20 00:18:41.000000 dom_tokenizers-0.0.8/tests/util.py
```

### Comparing `dom_tokenizers-0.0.7/LICENSE` & `dom_tokenizers-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.7/PKG-INFO` & `dom_tokenizers-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dom-tokenizers
-Version: 0.0.7
+Version: 0.0.8
 Summary: DOM-aware tokenizers for 🤗 Hugging Face language models
 Author: Gary Benson
 License: Apache-2.0
 Project-URL: Source, https://github.com/gbenson/dom-tokenizers
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dom-tokenizers Version: 0.0.7 Summary: DOM-aware
+Metadata-Version: 2.1 Name: dom-tokenizers Version: 0.0.8 Summary: DOM-aware
 tokenizers for ð¤Â HuggingÂ Face language models Author: Gary Benson License:
 Apache-2.0 Project-URL: Source, https://github.com/gbenson/dom-tokenizers
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

### Comparing `dom_tokenizers-0.0.7/README.md` & `dom_tokenizers-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.7/pyproject.toml` & `dom_tokenizers-0.0.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dom-tokenizers"
-version = "0.0.7"
+version = "0.0.8"
 authors = [{ name = "Gary Benson" }]
 description = "DOM-aware tokenizers for 🤗 Hugging Face language models"
 readme = "README.md"
 license = { text = "Apache-2.0" }
 requires-python = ">=3.10"  # match..case
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -45,14 +45,15 @@
     "datasets",
     "pillow",
 ]
 
 [project.scripts]
 train-tokenizer = "dom_tokenizers.train:main"
 dump-tokenizations = "dom_tokenizers.dump:main"
+tokenizer-diff = "dom_tokenizers.diff:main"
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.pytest.ini_options]
 addopts = "--cov=dom_tokenizers"
```

### Comparing `dom_tokenizers-0.0.7/src/dom_tokenizers/dump.py` & `dom_tokenizers-0.0.8/src/dom_tokenizers/dump.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import json
 import warnings
 
 from argparse import ArgumentParser
 
 from datasets import load_dataset
-from tokenizers.pre_tokenizers import PreTokenizer
 
-from .internal.transformers import AutoTokenizer
-from .pre_tokenizers import DOMSnapshotPreTokenizer
+from .tokenizers import DOMSnapshotTokenizer
 
 DEFAULT_DATASET = "gbenson/interesting-dom-snapshots"
 DEFAULT_SPLIT = "train"
 SEND_BUGS_TO = "https://github.com/gbenson/dom-tokenizers/issues"
 
 
 def main():
@@ -27,17 +25,15 @@
     parser.add_argument(
         "-s", "--split", metavar="SPLIT", default=DEFAULT_SPLIT,
         help=f"split of the dataset to tokenize [default: {DEFAULT_SPLIT}]")
     args = parser.parse_args()
 
     warnings.filterwarnings("ignore", message=r".*resume_download.*")
 
-    tokenizer = AutoTokenizer.from_pretrained(args.tokenizer)
-    tokenizer.backend_tokenizer.pre_tokenizer = \
-        PreTokenizer.custom(DOMSnapshotPreTokenizer())
+    tokenizer = DOMSnapshotTokenizer.from_pretrained(args.tokenizer)
 
     dataset = load_dataset(args.dataset, split=args.split)
     rows = ((row["source_index"], row["dom_snapshot"]) for row in dataset)
     rows = ((si, ss, json.dumps(ss, separators=(",", ":"))) for si, ss in rows)
     rows = ((len(ser), si, ss, ser) for si, ss, ser in rows)
     for _, source_index, dom_snapshot, serialized in sorted(rows):
         print(json.dumps(dict(
```

### Comparing `dom_tokenizers-0.0.7/src/dom_tokenizers/internal/transformers.py` & `dom_tokenizers-0.0.8/src/dom_tokenizers/internal/transformers.py`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.7/src/dom_tokenizers/pre_tokenizers/dom_snapshot.py` & `dom_tokenizers-0.0.8/src/dom_tokenizers/pre_tokenizers/dom_snapshot.py`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.7/src/dom_tokenizers/train.py` & `dom_tokenizers-0.0.8/src/dom_tokenizers/train.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 import os
 import warnings
 
 from argparse import ArgumentParser
 from math import log10, floor
 
 from datasets import load_dataset
-from tokenizers.pre_tokenizers import PreTokenizer, WhitespaceSplit
+from tokenizers.pre_tokenizers import WhitespaceSplit
 
-from .internal.transformers import AutoTokenizer
-from .pre_tokenizers import DOMSnapshotPreTokenizer
+from .tokenizers import DOMSnapshotTokenizer
 
 DEFAULT_BASE_TOKENIZER = "bert-base-cased"
 DEFAULT_SPLIT = "train"
 DEFAULT_SIZE = 1024
 SEND_BUGS_TO = "https://github.com/gbenson/dom-tokenizers/issues"
 
 
@@ -21,46 +20,45 @@
         training_dataset,
         base_tokenizer=DEFAULT_BASE_TOKENIZER,
         vocab_size=DEFAULT_SIZE,
         corpus_size=None):
 
     # Create the base tokenizer we'll train our new tokenizer from.
     if isinstance(base_tokenizer, str):
-        base_tokenizer = AutoTokenizer.from_pretrained(base_tokenizer)
-
-    # Create the custom pretokenizer our new tokenizer will use.
-    new_pretokenizer = DOMSnapshotPreTokenizer()
-
-    # List the custom special tokens that need adding to our tokenizer.
-    new_special_tokens = [
-        special_token
-        for special_token in new_pretokenizer.special_tokens
-        if base_tokenizer.tokenize(special_token) != [special_token]
-    ]
+        base_tokenizer = DOMSnapshotTokenizer.from_pretrained(
+            base_tokenizer)
 
     # It's not possible to train using a custom pre-tokenizer, the Rust
     # code raises "Exception: Custom PreTokenizer cannot be serialized"
     # (see https://github.com/huggingface/tokenizers/issues/269) so we
     # have to run our pre-tokenizer manually, then join its output with
     # whitespace and hope the regular pretokenizer takes it back apart
     # how we need it to.
 
+    new_pretokenizer = base_tokenizer.backend_tokenizer.pre_tokenizer
     base_tokenizer.backend_tokenizer.pre_tokenizer = WhitespaceSplit()
     base_pretokenizer = base_tokenizer.backend_tokenizer.pre_tokenizer
-    new_pretokenizer = PreTokenizer.custom(new_pretokenizer)
 
     def futz_input(real_input):
         pretokenized = new_pretokenizer.pre_tokenize_str(real_input)
         want_tokens = [token for token, offsets in pretokenized]
         futzed_input = " ".join(want_tokens)
         pretokenized = base_pretokenizer.pre_tokenize_str(futzed_input)
         got_tokens = [token for token, offsets in pretokenized]
         assert got_tokens == want_tokens
         return futzed_input
 
+    # List the custom special tokens that need adding to our tokenizer.
+    dom_snapshot_pre_tokenizer = base_tokenizer.backend_pre_tokenizer
+    new_special_tokens = [
+        special_token
+        for special_token in dom_snapshot_pre_tokenizer.special_tokens
+        if base_tokenizer.tokenize(special_token) != [special_token]
+    ]
+
     def get_training_corpus():
         for row in training_dataset:
             yield futz_input(json.dumps(row["dom_snapshot"]))
 
     # Try and get a dataset length, for the progress tracker.
     if corpus_size is None:
         try:
```

### Comparing `dom_tokenizers-0.0.7/src/dom_tokenizers.egg-info/SOURCES.txt` & `dom_tokenizers-0.0.8/src/dom_tokenizers.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 .flake8
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 src/dom_tokenizers/__init__.py
+src/dom_tokenizers/diff.py
 src/dom_tokenizers/dump.py
+src/dom_tokenizers/tokenizers.py
 src/dom_tokenizers/train.py
 src/dom_tokenizers/internal/__init__.py
 src/dom_tokenizers/internal/transformers.py
 src/dom_tokenizers/pre_tokenizers/__init__.py
 src/dom_tokenizers/pre_tokenizers/dom_snapshot.py
 tests/__init__.py
 tests/conftest.py
```

### Comparing `dom_tokenizers-0.0.7/tests/pre_tokenizers/dom_snapshot/conftest.py` & `dom_tokenizers-0.0.8/tests/pre_tokenizers/dom_snapshot/conftest.py`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.7/tests/pre_tokenizers/dom_snapshot/test_pre_tokenizer.py` & `dom_tokenizers-0.0.8/tests/pre_tokenizers/dom_snapshot/test_pre_tokenizer.py`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.7/tests/resources/raw-browser-response.json` & `dom_tokenizers-0.0.8/tests/resources/raw-browser-response.json`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.7/tests/resources/svg-in-base64.html` & `dom_tokenizers-0.0.8/tests/resources/svg-in-base64.html`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.7/tests/resources/svg-in-base64.json` & `dom_tokenizers-0.0.8/tests/resources/svg-in-base64.json`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.7/tests/test_train_tokenizer.py` & `dom_tokenizers-0.0.8/tests/test_train_tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from datasets import Dataset
 
 from dom_tokenizers.train import train_tokenizer
 
 from .util import load_resource
 
 
-def test_base64(base_tokenizer, dom_snapshot_pre_tokenizer):
+def test_base64(dom_snapshot_pre_tokenizer):
     """Test that base64 is entered successfully.  Incorrectly-sequenced
     lowercasing (i.e. applied prior to pre-tokenization) will cause this
     test to fail.
     """
     snapshot = load_resource("svg-in-base64.json")
     tokenizer = train_tokenizer(
         training_dataset=Dataset.from_dict({
```

### Comparing `dom_tokenizers-0.0.7/tests/util.py` & `dom_tokenizers-0.0.8/tests/util.py`

 * *Files identical despite different names*

