# Comparing `tmp/starfile-0.5.7.tar.gz` & `tmp/starfile-0.5.8.tar.gz`

## Comparing `starfile-0.5.7.tar` & `starfile-0.5.8.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 starfile-0.5.7/.copier-answers.yml
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 starfile-0.5.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 starfile-0.5.7/mkdocs.yml
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 starfile-0.5.7/setup.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 starfile-0.5.7/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 starfile-0.5.7/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 starfile-0.5.7/.github/dependabot.yml
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 starfile-0.5.7/.github/workflows/build-and-deploy-docs.yml
--rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 starfile-0.5.7/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 starfile-0.5.7/docs/index.md
--rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 starfile-0.5.7/docs/examples/merging.md
--rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 starfile-0.5.7/docs/examples/multi_block.md
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 starfile-0.5.7/docs/examples/single_block.md
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 starfile-0.5.7/src/starfile/__init__.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 starfile-0.5.7/src/starfile/__main__.py
--rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 starfile-0.5.7/src/starfile/functions.py
--rw-r--r--   0        0        0     5966 2020-02-02 00:00:00.000000 starfile-0.5.7/src/starfile/parser.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 starfile-0.5.7/src/starfile/typing.py
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 starfile-0.5.7/src/starfile/utils.py
--rw-r--r--   0        0        0     5866 2020-02-02 00:00:00.000000 starfile-0.5.7/src/starfile/writer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starfile-0.5.7/tests/__init__.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 starfile-0.5.7/tests/constants.py
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 starfile-0.5.7/tests/test_functional_interface.py
--rw-r--r--   0        0        0     8960 2020-02-02 00:00:00.000000 starfile-0.5.7/tests/test_parsing.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 starfile-0.5.7/tests/test_read_write_round_trip.py
--rw-r--r--   0        0        0     4025 2020-02-02 00:00:00.000000 starfile-0.5.7/tests/test_writing.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 starfile-0.5.7/tests/utils.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 starfile-0.5.7/tests/data/basic_double_quote.star
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 starfile-0.5.7/tests/data/basic_single_quote.star
--rw-r--r--   0        0        0    12768 2020-02-02 00:00:00.000000 starfile-0.5.7/tests/data/default_pipeline.star
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 starfile-0.5.7/tests/data/empty_loop.star
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 starfile-0.5.7/tests/data/loop_double_quote.star
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 starfile-0.5.7/tests/data/loop_single_quote.star
--rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 starfile-0.5.7/tests/data/one_loop.star
--rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 starfile-0.5.7/tests/data/postprocess.star
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 starfile-0.5.7/tests/data/rln3.1_data_style.star
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 starfile-0.5.7/tests/data/single_line_end_of_multiblock.star
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 starfile-0.5.7/tests/data/single_line_middle_of_multiblock.star
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 starfile-0.5.7/tests/data/two_basic_blocks.star
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 starfile-0.5.7/tests/data/two_single_line_loop_blocks.star
--rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 starfile-0.5.7/tests/data/relion_tutorial/run_it025_optimiser_2D.star
--rw-r--r--   0        0        0     6251 2020-02-02 00:00:00.000000 starfile-0.5.7/tests/data/relion_tutorial/run_it025_optimiser_3D.star
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 starfile-0.5.7/tests/data/relion_tutorial/run_it025_sampling_2D.star
--rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 starfile-0.5.7/tests/data/relion_tutorial/run_it025_sampling_3D.star
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 starfile-0.5.7/.gitignore
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 starfile-0.5.7/LICENSE
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 starfile-0.5.7/README.md
--rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 starfile-0.5.7/pyproject.toml
--rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 starfile-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 starfile-0.5.8/.copier-answers.yml
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 starfile-0.5.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 starfile-0.5.8/mkdocs.yml
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 starfile-0.5.8/setup.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 starfile-0.5.8/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 starfile-0.5.8/.github/TEST_FAIL_TEMPLATE.md
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 starfile-0.5.8/.github/dependabot.yml
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 starfile-0.5.8/.github/workflows/build-and-deploy-docs.yml
+-rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 starfile-0.5.8/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 starfile-0.5.8/docs/index.md
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 starfile-0.5.8/docs/examples/merging.md
+-rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 starfile-0.5.8/docs/examples/multi_block.md
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 starfile-0.5.8/docs/examples/single_block.md
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 starfile-0.5.8/src/starfile/__init__.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 starfile-0.5.8/src/starfile/__main__.py
+-rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 starfile-0.5.8/src/starfile/functions.py
+-rw-r--r--   0        0        0     6014 2020-02-02 00:00:00.000000 starfile-0.5.8/src/starfile/parser.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 starfile-0.5.8/src/starfile/typing.py
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 starfile-0.5.8/src/starfile/utils.py
+-rw-r--r--   0        0        0     5866 2020-02-02 00:00:00.000000 starfile-0.5.8/src/starfile/writer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starfile-0.5.8/tests/__init__.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 starfile-0.5.8/tests/constants.py
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 starfile-0.5.8/tests/test_functional_interface.py
+-rw-r--r--   0        0        0     8960 2020-02-02 00:00:00.000000 starfile-0.5.8/tests/test_parsing.py
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 starfile-0.5.8/tests/test_read_write_round_trip.py
+-rw-r--r--   0        0        0     4025 2020-02-02 00:00:00.000000 starfile-0.5.8/tests/test_writing.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 starfile-0.5.8/tests/utils.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 starfile-0.5.8/tests/data/basic_double_quote.star
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 starfile-0.5.8/tests/data/basic_single_quote.star
+-rw-r--r--   0        0        0    12768 2020-02-02 00:00:00.000000 starfile-0.5.8/tests/data/default_pipeline.star
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 starfile-0.5.8/tests/data/empty_loop.star
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 starfile-0.5.8/tests/data/loop_double_quote.star
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 starfile-0.5.8/tests/data/loop_single_quote.star
+-rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 starfile-0.5.8/tests/data/one_loop.star
+-rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 starfile-0.5.8/tests/data/postprocess.star
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 starfile-0.5.8/tests/data/rln3.1_data_style.star
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 starfile-0.5.8/tests/data/single_line_end_of_multiblock.star
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 starfile-0.5.8/tests/data/single_line_middle_of_multiblock.star
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 starfile-0.5.8/tests/data/two_basic_blocks.star
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 starfile-0.5.8/tests/data/two_single_line_loop_blocks.star
+-rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 starfile-0.5.8/tests/data/relion_tutorial/run_it025_optimiser_2D.star
+-rw-r--r--   0        0        0     6251 2020-02-02 00:00:00.000000 starfile-0.5.8/tests/data/relion_tutorial/run_it025_optimiser_3D.star
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 starfile-0.5.8/tests/data/relion_tutorial/run_it025_sampling_2D.star
+-rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 starfile-0.5.8/tests/data/relion_tutorial/run_it025_sampling_3D.star
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 starfile-0.5.8/.gitignore
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 starfile-0.5.8/LICENSE
+-rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 starfile-0.5.8/README.md
+-rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 starfile-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 starfile-0.5.8/PKG-INFO
```

### Comparing `starfile-0.5.7/.pre-commit-config.yaml` & `starfile-0.5.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `starfile-0.5.7/mkdocs.yml` & `starfile-0.5.8/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `starfile-0.5.7/.github/workflows/build-and-deploy-docs.yml` & `starfile-0.5.8/.github/workflows/build-and-deploy-docs.yml`

 * *Files identical despite different names*

### Comparing `starfile-0.5.7/.github/workflows/ci.yml` & `starfile-0.5.8/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `starfile-0.5.7/docs/index.md` & `starfile-0.5.8/docs/index.md`

 * *Files identical despite different names*

### Comparing `starfile-0.5.7/docs/examples/merging.md` & `starfile-0.5.8/docs/examples/merging.md`

 * *Files identical despite different names*

### Comparing `starfile-0.5.7/docs/examples/multi_block.md` & `starfile-0.5.8/docs/examples/multi_block.md`

 * *Files identical despite different names*

### Comparing `starfile-0.5.7/docs/examples/single_block.md` & `starfile-0.5.8/docs/examples/single_block.md`

 * *Files identical despite different names*

### Comparing `starfile-0.5.7/src/starfile/__main__.py` & `starfile-0.5.8/src/starfile/__main__.py`

 * *Files identical despite different names*

### Comparing `starfile-0.5.7/src/starfile/functions.py` & `starfile-0.5.8/src/starfile/functions.py`

 * *Files identical despite different names*

### Comparing `starfile-0.5.7/src/starfile/parser.py` & `starfile-0.5.8/src/starfile/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import linecache
 from collections import deque
 from io import StringIO
 from linecache import getline
 import shlex
 
 import numpy as np
 import pandas as pd
@@ -41,14 +42,15 @@
         self.n_lines_in_file = count_lines(self.filename)
         self.n_blocks_to_read = n_blocks_to_read
         self.parse_as_string = parse_as_string
 
         # parse file
         self.current_line_number = 0
         self.parse_file()
+        linecache.clearcache()
 
     @property
     def current_line(self) -> str:
         return getline(str(self.filename), self.current_line_number).strip()
 
     def parse_file(self):
         while self.current_line_number <= self.n_lines_in_file:
```

### Comparing `starfile-0.5.7/src/starfile/utils.py` & `starfile-0.5.8/src/starfile/utils.py`

 * *Files identical despite different names*

### Comparing `starfile-0.5.7/src/starfile/writer.py` & `starfile-0.5.8/src/starfile/writer.py`

 * *Files identical despite different names*

### Comparing `starfile-0.5.7/tests/constants.py` & `starfile-0.5.8/tests/constants.py`

 * *Files identical despite different names*

### Comparing `starfile-0.5.7/tests/test_functional_interface.py` & `starfile-0.5.8/tests/test_functional_interface.py`

 * *Files identical despite different names*

### Comparing `starfile-0.5.7/tests/test_parsing.py` & `starfile-0.5.8/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `starfile-0.5.7/tests/test_writing.py` & `starfile-0.5.8/tests/test_writing.py`

 * *Files identical despite different names*

### Comparing `starfile-0.5.7/tests/data/default_pipeline.star` & `starfile-0.5.8/tests/data/default_pipeline.star`

 * *Files identical despite different names*

### Comparing `starfile-0.5.7/tests/data/one_loop.star` & `starfile-0.5.8/tests/data/one_loop.star`

 * *Files identical despite different names*

### Comparing `starfile-0.5.7/tests/data/postprocess.star` & `starfile-0.5.8/tests/data/postprocess.star`

 * *Files identical despite different names*

### Comparing `starfile-0.5.7/tests/data/rln3.1_data_style.star` & `starfile-0.5.8/tests/data/rln3.1_data_style.star`

 * *Files identical despite different names*

### Comparing `starfile-0.5.7/tests/data/single_line_end_of_multiblock.star` & `starfile-0.5.8/tests/data/single_line_end_of_multiblock.star`

 * *Files identical despite different names*

### Comparing `starfile-0.5.7/tests/data/relion_tutorial/run_it025_optimiser_2D.star` & `starfile-0.5.8/tests/data/relion_tutorial/run_it025_optimiser_2D.star`

 * *Files identical despite different names*

### Comparing `starfile-0.5.7/tests/data/relion_tutorial/run_it025_optimiser_3D.star` & `starfile-0.5.8/tests/data/relion_tutorial/run_it025_optimiser_3D.star`

 * *Files identical despite different names*

### Comparing `starfile-0.5.7/tests/data/relion_tutorial/run_it025_sampling_2D.star` & `starfile-0.5.8/tests/data/relion_tutorial/run_it025_sampling_2D.star`

 * *Files identical despite different names*

### Comparing `starfile-0.5.7/tests/data/relion_tutorial/run_it025_sampling_3D.star` & `starfile-0.5.8/tests/data/relion_tutorial/run_it025_sampling_3D.star`

 * *Files identical despite different names*

### Comparing `starfile-0.5.7/LICENSE` & `starfile-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `starfile-0.5.7/README.md` & `starfile-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `starfile-0.5.7/pyproject.toml` & `starfile-0.5.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `starfile-0.5.7/PKG-INFO` & `starfile-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: starfile
-Version: 0.5.7
+Version: 0.5.8
 Summary: STAR file I/O in Python
 Project-URL: homepage, https://github.com/teamtomo/starfile
 Project-URL: repository, https://github.com/teamtomo/starfile
 Author-email: Alister Burt <alisterburt@gmail.com>
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
```

