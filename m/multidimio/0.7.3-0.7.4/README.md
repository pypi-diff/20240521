# Comparing `tmp/multidimio-0.7.3.tar.gz` & `tmp/multidimio-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multidimio-0.7.3.tar", max compression
+gzip compressed data, was "multidimio-0.7.4.tar", max compression
```

## Comparing `multidimio-0.7.3.tar` & `multidimio-0.7.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    10203 2024-04-04 15:57:28.082587 multidimio-0.7.3/LICENSE
--rw-r--r--   0        0        0     6028 2024-04-04 15:57:28.082587 multidimio-0.7.3/README.md
--rw-r--r--   0        0        0     2747 2024-04-04 15:57:37.502619 multidimio-0.7.3/pyproject.toml
--rw-r--r--   0        0        0      474 2024-04-04 15:57:28.094587 multidimio-0.7.3/src/mdio/__init__.py
--rw-r--r--   0        0        0     2954 2024-04-04 15:57:28.094587 multidimio-0.7.3/src/mdio/__main__.py
--rw-r--r--   0        0        0      127 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/api/__init__.py
--rw-r--r--   0        0        0    25195 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/api/accessor.py
--rw-r--r--   0        0        0     8520 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/api/convenience.py
--rw-r--r--   0        0        0     4451 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/api/io_utils.py
--rw-r--r--   0        0        0      105 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/commands/__init__.py
--rw-r--r--   0        0        0     2246 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/commands/copy.py
--rw-r--r--   0        0        0     5007 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/commands/info.py
--rw-r--r--   0        0        0    14703 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/commands/segy.py
--rw-r--r--   0        0        0      529 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/constants.py
--rw-r--r--   0        0        0      141 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/converters/__init__.py
--rw-r--r--   0        0        0     1485 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/converters/exceptions.py
--rw-r--r--   0        0        0     6510 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/converters/mdio.py
--rw-r--r--   0        0        0    20972 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/converters/segy.py
--rw-r--r--   0        0        0      143 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/core/__init__.py
--rw-r--r--   0        0        0     3811 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/core/dimension.py
--rw-r--r--   0        0        0      268 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/core/exceptions.py
--rw-r--r--   0        0        0     3694 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/core/grid.py
--rw-r--r--   0        0        0     2917 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/core/indexing.py
--rw-r--r--   0        0        0     2727 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/core/serialization.py
--rw-r--r--   0        0        0      429 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/core/utils_write.py
--rw-r--r--   0        0        0     1646 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/py.typed
--rw-r--r--   0        0        0       44 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/segy/__init__.py
--rw-r--r--   0        0        0      636 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/segy/_standards_common.py
--rw-r--r--   0        0        0     9384 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/segy/_standards_rev0.py
--rw-r--r--   0        0        0     8514 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/segy/_workers.py
--rw-r--r--   0        0        0    11128 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/segy/blocked_io.py
--rw-r--r--   0        0        0     2048 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/segy/byte_utils.py
--rw-r--r--   0        0        0     9408 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/segy/creation.py
--rw-r--r--   0        0        0     4856 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/segy/ebcdic.py
--rw-r--r--   0        0        0     1946 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/segy/exceptions.py
--rw-r--r--   0        0        0    23385 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/segy/geometry.py
--rw-r--r--   0        0        0     2748 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/segy/headers.py
--rw-r--r--   0        0        0     3561 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/segy/headers_text.py
--rw-r--r--   0        0        0     1118 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/segy/helpers_segy.py
--rw-r--r--   0        0        0     5785 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/segy/ibm_float.py
--rw-r--r--   0        0        0     4958 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/segy/parsers.py
--rw-r--r--   0        0        0     5532 2024-04-04 15:57:28.098587 multidimio-0.7.3/src/mdio/segy/utilities.py
--rw-r--r--   0        0        0     7834 1970-01-01 00:00:00.000000 multidimio-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0    10203 2024-05-21 19:15:39.175093 multidimio-0.7.4/LICENSE
+-rw-r--r--   0        0        0     6028 2024-05-21 19:15:39.179093 multidimio-0.7.4/README.md
+-rw-r--r--   0        0        0     2746 2024-05-21 19:15:48.583216 multidimio-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0      473 2024-05-21 19:15:39.191093 multidimio-0.7.4/src/mdio/__init__.py
+-rw-r--r--   0        0        0     2953 2024-05-21 19:15:39.191093 multidimio-0.7.4/src/mdio/__main__.py
+-rw-r--r--   0        0        0      126 2024-05-21 19:15:39.191093 multidimio-0.7.4/src/mdio/api/__init__.py
+-rw-r--r--   0        0        0    25195 2024-05-21 19:15:39.191093 multidimio-0.7.4/src/mdio/api/accessor.py
+-rw-r--r--   0        0        0     8520 2024-05-21 19:15:39.191093 multidimio-0.7.4/src/mdio/api/convenience.py
+-rw-r--r--   0        0        0     4450 2024-05-21 19:15:39.191093 multidimio-0.7.4/src/mdio/api/io_utils.py
+-rw-r--r--   0        0        0      105 2024-05-21 19:15:39.191093 multidimio-0.7.4/src/mdio/commands/__init__.py
+-rw-r--r--   0        0        0     2245 2024-05-21 19:15:39.191093 multidimio-0.7.4/src/mdio/commands/copy.py
+-rw-r--r--   0        0        0     5007 2024-05-21 19:15:39.191093 multidimio-0.7.4/src/mdio/commands/info.py
+-rw-r--r--   0        0        0    14702 2024-05-21 19:15:39.191093 multidimio-0.7.4/src/mdio/commands/segy.py
+-rw-r--r--   0        0        0      528 2024-05-21 19:15:39.191093 multidimio-0.7.4/src/mdio/constants.py
+-rw-r--r--   0        0        0      140 2024-05-21 19:15:39.191093 multidimio-0.7.4/src/mdio/converters/__init__.py
+-rw-r--r--   0        0        0     1485 2024-05-21 19:15:39.191093 multidimio-0.7.4/src/mdio/converters/exceptions.py
+-rw-r--r--   0        0        0     6820 2024-05-21 19:15:39.191093 multidimio-0.7.4/src/mdio/converters/mdio.py
+-rw-r--r--   0        0        0    20971 2024-05-21 19:15:39.191093 multidimio-0.7.4/src/mdio/converters/segy.py
+-rw-r--r--   0        0        0      142 2024-05-21 19:15:39.191093 multidimio-0.7.4/src/mdio/core/__init__.py
+-rw-r--r--   0        0        0     3810 2024-05-21 19:15:39.191093 multidimio-0.7.4/src/mdio/core/dimension.py
+-rw-r--r--   0        0        0      267 2024-05-21 19:15:39.191093 multidimio-0.7.4/src/mdio/core/exceptions.py
+-rw-r--r--   0        0        0     3693 2024-05-21 19:15:39.191093 multidimio-0.7.4/src/mdio/core/grid.py
+-rw-r--r--   0        0        0     2916 2024-05-21 19:15:39.191093 multidimio-0.7.4/src/mdio/core/indexing.py
+-rw-r--r--   0        0        0     2726 2024-05-21 19:15:39.191093 multidimio-0.7.4/src/mdio/core/serialization.py
+-rw-r--r--   0        0        0      428 2024-05-21 19:15:39.191093 multidimio-0.7.4/src/mdio/core/utils_write.py
+-rw-r--r--   0        0        0     1645 2024-05-21 19:15:39.191093 multidimio-0.7.4/src/mdio/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-21 19:15:39.191093 multidimio-0.7.4/src/mdio/py.typed
+-rw-r--r--   0        0        0       44 2024-05-21 19:15:39.191093 multidimio-0.7.4/src/mdio/segy/__init__.py
+-rw-r--r--   0        0        0      635 2024-05-21 19:15:39.191093 multidimio-0.7.4/src/mdio/segy/_standards_common.py
+-rw-r--r--   0        0        0     9383 2024-05-21 19:15:39.191093 multidimio-0.7.4/src/mdio/segy/_standards_rev0.py
+-rw-r--r--   0        0        0     8513 2024-05-21 19:15:39.191093 multidimio-0.7.4/src/mdio/segy/_workers.py
+-rw-r--r--   0        0        0    11195 2024-05-21 19:15:39.191093 multidimio-0.7.4/src/mdio/segy/blocked_io.py
+-rw-r--r--   0        0        0     2047 2024-05-21 19:15:39.191093 multidimio-0.7.4/src/mdio/segy/byte_utils.py
+-rw-r--r--   0        0        0     9407 2024-05-21 19:15:39.195093 multidimio-0.7.4/src/mdio/segy/creation.py
+-rw-r--r--   0        0        0     4855 2024-05-21 19:15:39.195093 multidimio-0.7.4/src/mdio/segy/ebcdic.py
+-rw-r--r--   0        0        0     1945 2024-05-21 19:15:39.195093 multidimio-0.7.4/src/mdio/segy/exceptions.py
+-rw-r--r--   0        0        0    23385 2024-05-21 19:15:39.195093 multidimio-0.7.4/src/mdio/segy/geometry.py
+-rw-r--r--   0        0        0     2747 2024-05-21 19:15:39.195093 multidimio-0.7.4/src/mdio/segy/headers.py
+-rw-r--r--   0        0        0     3560 2024-05-21 19:15:39.195093 multidimio-0.7.4/src/mdio/segy/headers_text.py
+-rw-r--r--   0        0        0     1117 2024-05-21 19:15:39.195093 multidimio-0.7.4/src/mdio/segy/helpers_segy.py
+-rw-r--r--   0        0        0     5784 2024-05-21 19:15:39.195093 multidimio-0.7.4/src/mdio/segy/ibm_float.py
+-rw-r--r--   0        0        0     4957 2024-05-21 19:15:39.195093 multidimio-0.7.4/src/mdio/segy/parsers.py
+-rw-r--r--   0        0        0     5531 2024-05-21 19:15:39.195093 multidimio-0.7.4/src/mdio/segy/utilities.py
+-rw-r--r--   0        0        0     7834 1970-01-01 00:00:00.000000 multidimio-0.7.4/PKG-INFO
```

### Comparing `multidimio-0.7.3/LICENSE` & `multidimio-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.3/README.md` & `multidimio-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.3/pyproject.toml` & `multidimio-0.7.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "multidimio"
-version = "0.7.3"
+version = "0.7.4"
 description = "Cloud-native, scalable, and user-friendly multi dimensional energy data!"
 authors = ["TGS <sys-opensource@tgs.com>"]
 maintainers = [
     "Altay Sansal <altay.sansal@tgs.com>",
 ]
 license = "Apache-2.0"
 readme = "README.md"
@@ -46,15 +46,15 @@
 
 [tool.poetry.extras]
 distributed = ["distributed", "bokeh"]
 cloud = ["s3fs", "gcsfs", "adlfs"]
 lossy = ["zfpy"]
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.12.1"
+black = "^24.4.2"
 coverage = {version = "^7.4.0", extras = ["toml"]}
 darglint = "^1.8.1"
 flake8 = "^7.0.0"
 flake8-bandit = "^4.1.1"
 flake8-bugbear = "^23.12.2"
 flake8-docstrings = "^1.7.0"
 flake8-rst-docstrings = "^0.3.0"
```

### Comparing `multidimio-0.7.3/src/mdio/__main__.py` & `multidimio-0.7.4/src/mdio/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Command-line interface."""
 
-
 from __future__ import annotations
 
 import importlib
 from importlib import metadata
 from pathlib import Path
 from typing import Callable
```

### Comparing `multidimio-0.7.3/src/mdio/api/accessor.py` & `multidimio-0.7.4/src/mdio/api/accessor.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.3/src/mdio/api/convenience.py` & `multidimio-0.7.4/src/mdio/api/convenience.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.3/src/mdio/api/io_utils.py` & `multidimio-0.7.4/src/mdio/api/io_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Utilities related to API functions and classes."""
 
-
 from __future__ import annotations
 
 from typing import Any
 
 import dask.array as da
 import zarr
 from zarr.storage import FSStore
```

### Comparing `multidimio-0.7.3/src/mdio/commands/copy.py` & `multidimio-0.7.4/src/mdio/commands/copy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """MDIO Dataset copy command."""
 
-
 from __future__ import annotations
 
 from click import STRING
 from click import argument
 from click import command
 from click import option
 from click_params import JSON
```

### Comparing `multidimio-0.7.3/src/mdio/commands/info.py` & `multidimio-0.7.4/src/mdio/commands/info.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.3/src/mdio/commands/segy.py` & `multidimio-0.7.4/src/mdio/commands/segy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """SEG-Y Import/Export CLI Plugin."""
 
-
 from typing import Any
 
 from click import BOOL
 from click import FLOAT
 from click import STRING
 from click import Choice
 from click import Group
```

### Comparing `multidimio-0.7.3/src/mdio/constants.py` & `multidimio-0.7.4/src/mdio/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Constant values used across MDIO."""
 
-
 import numpy as np
 
 
 FLOAT16_MAX = np.finfo("float16").max
 FLOAT16_MIN = np.finfo("float16").min
 
 FLOAT32_MAX = np.finfo("float32").max
```

### Comparing `multidimio-0.7.3/src/mdio/converters/exceptions.py` & `multidimio-0.7.4/src/mdio/converters/exceptions.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.7.3/src/mdio/converters/mdio.py` & `multidimio-0.7.4/src/mdio/converters/mdio.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Conversion from to MDIO various other formats."""
 
-
 from __future__ import annotations
 
+import os
 from os import path
 from tempfile import TemporaryDirectory
 
 import numpy as np
+from psutil import cpu_count
 from tqdm.dask import TqdmCallback
 
 from mdio import MDIOReader
 from mdio.segy.blocked_io import to_segy
 from mdio.segy.byte_utils import ByteOrder
 from mdio.segy.byte_utils import Dtype
 from mdio.segy.creation import concat_files
@@ -20,14 +21,18 @@
 
 try:
     import distributed
 except ImportError:
     distributed = None
 
 
+default_cpus = cpu_count(logical=True)
+NUM_CPUS = int(os.getenv("MDIO__EXPORT__CPU_COUNT", default_cpus))
+
+
 def mdio_to_segy(  # noqa: C901
     mdio_path_or_buffer: str,
     output_segy_path: str,
     endian: str = "big",
     access_pattern: str = "012",
     out_sample_format: str = "ibm32",
     storage_options: dict = None,
@@ -172,15 +177,20 @@
                 samples=samples,
                 headers=headers,
                 live_mask=live_mask,
                 out_dtype=out_dtype,
                 out_byteorder=out_byteorder,
                 file_root=tmp_dir.name,
                 axis=tuple(range(1, samples.ndim)),
-            ).compute()
+            )
+
+            if client is not None:
+                flat_files = flat_files.compute()
+            else:
+                flat_files = flat_files.compute(num_workers=NUM_CPUS)
 
         # If whole blocks are missing, remove them from the list.
         missing_mask = flat_files == "missing"
         flat_files = flat_files[~missing_mask]
 
         final_concat = [output_segy_path] + flat_files.tolist()
```

### Comparing `multidimio-0.7.3/src/mdio/converters/segy.py` & `multidimio-0.7.4/src/mdio/converters/segy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Conversion from SEG-Y to MDIO."""
 
-
 from __future__ import annotations
 
 import logging
 import os
 from datetime import datetime
 from datetime import timezone
 from importlib import metadata
```

### Comparing `multidimio-0.7.3/src/mdio/core/dimension.py` & `multidimio-0.7.4/src/mdio/core/dimension.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Dimension (grid) abstraction and serializers."""
 
-
 from __future__ import annotations
 
 import inspect
 from dataclasses import dataclass
 from typing import Any
 
 import numpy as np
```

### Comparing `multidimio-0.7.3/src/mdio/core/grid.py` & `multidimio-0.7.4/src/mdio/core/grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Grid abstraction with serializers."""
 
-
 from __future__ import annotations
 
 import inspect
 from dataclasses import dataclass
 
 import numpy as np
 import zarr
```

### Comparing `multidimio-0.7.3/src/mdio/core/indexing.py` & `multidimio-0.7.4/src/mdio/core/indexing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Indexing logic."""
 
-
 import itertools
 from math import ceil
 
 import numpy as np
 from zarr import Array
```

### Comparing `multidimio-0.7.3/src/mdio/core/serialization.py` & `multidimio-0.7.4/src/mdio/core/serialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """(De)serialization factory design pattern.
 
 Current support for JSON and YAML.
 """
 
-
 import json
 from abc import ABC
 from abc import abstractmethod
 from inspect import Signature
 from typing import Callable
 
 import yaml
```

### Comparing `multidimio-0.7.3/src/mdio/exceptions.py` & `multidimio-0.7.4/src/mdio/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Custom exceptions related to MDIO functionality."""
 
-
 from __future__ import annotations
 
 
 class MDIOError(Exception):
     """Base exceptions class."""
```

### Comparing `multidimio-0.7.3/src/mdio/segy/_standards_common.py` & `multidimio-0.7.4/src/mdio/segy/_standards_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Common elements for SEG-Y standards datasets."""
 
-
 from enum import IntEnum
 
 
 class SegyFloatFormat(IntEnum):
     """Numeric type to SEG-Y code mapping."""
 
     IBM32 = 1
```

### Comparing `multidimio-0.7.3/src/mdio/segy/_standards_rev0.py` & `multidimio-0.7.4/src/mdio/segy/_standards_rev0.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """SEG-Y Rev 0 standard and its definitions."""
 
-
 from mdio.segy.byte_utils import ByteOrder
 from mdio.segy.byte_utils import Dtype
 from mdio.segy.byte_utils import OrderedType
 from mdio.segy.headers import Header
 from mdio.segy.headers import HeaderGroup
```

### Comparing `multidimio-0.7.3/src/mdio/segy/_workers.py` & `multidimio-0.7.4/src/mdio/segy/_workers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Low level workers for parsing and writing SEG-Y to Zarr."""
 
-
 from __future__ import annotations
 
 from typing import Any
 from typing import Sequence
 
 import numpy as np
 import segyio
```

### Comparing `multidimio-0.7.3/src/mdio/segy/blocked_io.py` & `multidimio-0.7.4/src/mdio/segy/blocked_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Functions for doing blocked I/O from SEG-Y."""
 
-
 from __future__ import annotations
 
 import multiprocessing as mp
+import os
 from concurrent.futures import ProcessPoolExecutor
 from itertools import repeat
 
 import numpy as np
 from dask.array import Array
 from dask.array import blockwise
 from dask.array.reductions import _tree_reduce
@@ -31,16 +31,16 @@
     import zfpy  # Base library
     from zarr import ZFPY  # Codec
 
 except ImportError:
     ZFPY = None
     zfpy = None
 
-# Globals
-NUM_CORES = cpu_count(logical=False)
+default_cpus = cpu_count(logical=True)
+NUM_CPUS = int(os.getenv("MDIO__IMPORT__CPU_COUNT", default_cpus))
 
 
 def to_zarr(
     segy_path: str,
     segy_endian: str,
     grid: Grid,
     data_root: Group,
@@ -132,15 +132,15 @@
     # Initialize chunk iterator (returns next chunk slice indices each iteration)
     chunker = ChunkIterator(trace_array, chunk_samples=False)
     num_chunks = len(chunker)
 
     # For Unix async writes with s3fs/fsspec & multiprocessing,
     # use 'spawn' instead of default 'fork' to avoid deadlocks
     # on cloud stores. Slower but necessary. Default on Windows.
-    num_workers = min(num_chunks, NUM_CORES)
+    num_workers = min(num_chunks, NUM_CPUS)
     context = mp.get_context("spawn")
     executor = ProcessPoolExecutor(max_workers=num_workers, mp_context=context)
 
     # Chunksize here is for multiprocessing, not Zarr chunksize.
     pool_chunksize, extra = divmod(num_chunks, num_workers * 4)
     pool_chunksize += 1 if extra else pool_chunksize
```

### Comparing `multidimio-0.7.3/src/mdio/segy/byte_utils.py` & `multidimio-0.7.4/src/mdio/segy/byte_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Module for custom struct abstraction utilities."""
 
-
 import sys
 from dataclasses import dataclass
 from enum import Enum
 
 import numpy as np
 from numpy.typing import NDArray
```

### Comparing `multidimio-0.7.3/src/mdio/segy/creation.py` & `multidimio-0.7.4/src/mdio/segy/creation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """SEG-Y creation utilities."""
 
-
 from __future__ import annotations
 
 import os
 from os import path
 from shutil import copyfileobj
 from time import sleep
 from uuid import uuid4
```

### Comparing `multidimio-0.7.3/src/mdio/segy/ebcdic.py` & `multidimio-0.7.4/src/mdio/segy/ebcdic.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     https://www.ibm.com/docs/en/iis/11.7?topic=tables-conversion-table-irregularities
     The pipe or vertical line operator "|" EBCDIC / ASCII Hex: 0x4F / 0x21 (instead of 0x7C per SEGY)
     * 0x4F is the integer 79.
     * If we get `EBCDIC_TO_ASCII[79]` then that maps to Hex `0x21` which is `33`.
     * Then reverse it and get `ASCII_TO_EBCDIC[33]` that maps back to `0x4F` which is "|".
 """
 
-
 import numpy as np
 
 
 # fmt: off
 ASCII_TO_EBCDIC = np.asarray(
     [
         0x00, 0x01, 0x02, 0x03, 0x37, 0x2D, 0x2E, 0x2F, 0x16, 0x05, 0x25, 0x0B, 0x0C, 0x0D, 0x0E, 0x0F,  # 15
```

### Comparing `multidimio-0.7.3/src/mdio/segy/exceptions.py` & `multidimio-0.7.4/src/mdio/segy/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Custom exceptions for SEG-Y."""
 
-
 from mdio.exceptions import MDIOError
 
 
 class InvalidSEGYFileError(MDIOError):
     """Raised when there is an IOError from segyio."""
```

### Comparing `multidimio-0.7.3/src/mdio/segy/geometry.py` & `multidimio-0.7.4/src/mdio/segy/geometry.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """SEG-Y geometry handling functions."""
 
-
 from __future__ import annotations
 
 import logging
 import time
 from abc import ABC
 from abc import abstractmethod
 from enum import Enum
@@ -74,14 +73,15 @@
         Gun 2 ->         1------------------20
 
     Configuration B:
         Gun 1 ->         1------------------39
         Gun 2 ->         2------------------40
 
     """
+
     A = auto()
     B = auto()
 
 
 def analyze_streamer_headers(
     index_headers: dict[str, npt.NDArray],
 ) -> tuple[npt.NDArray, npt.NDArray, npt.NDArray, StreamerShotGeometryType]:
```

### Comparing `multidimio-0.7.3/src/mdio/segy/headers.py` & `multidimio-0.7.4/src/mdio/segy/headers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """SEG-Y header abstractions."""
 
-
 from collections import abc
 from dataclasses import dataclass
 from dataclasses import field
 
 import numpy as np
 
 from mdio.segy.byte_utils import OrderedType
```

### Comparing `multidimio-0.7.3/src/mdio/segy/headers_text.py` & `multidimio-0.7.4/src/mdio/segy/headers_text.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Text header manipulation utilities."""
 
-
 from __future__ import annotations
 
 from typing import Sequence
 
 import numpy as np
 
 from mdio.segy.ebcdic import ASCII_TO_EBCDIC
```

### Comparing `multidimio-0.7.3/src/mdio/segy/helpers_segy.py` & `multidimio-0.7.4/src/mdio/segy/helpers_segy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Helper functions for tinkering with SEG-Y related Zarr."""
 
-
 from zarr import Group
 from zarr import open_group
 from zarr.errors import ContainsGroupError
 from zarr.storage import FSStore
 
 from mdio.core.exceptions import MDIOAlreadyExistsError
```

### Comparing `multidimio-0.7.3/src/mdio/segy/ibm_float.py` & `multidimio-0.7.4/src/mdio/segy/ibm_float.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Low-level floating point conversion operations."""
 
-
 import os
 
 import numba as nb
 import numpy as np
 
 
 # If Numba's JIT compilation is disabled, force vectorized
```

### Comparing `multidimio-0.7.3/src/mdio/segy/parsers.py` & `multidimio-0.7.4/src/mdio/segy/parsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Parsers for sections of SEG-Y files."""
 
-
 from __future__ import annotations
 
 from concurrent.futures import ProcessPoolExecutor
 from itertools import repeat
 from math import ceil
 from typing import Any
 from typing import Sequence
```

### Comparing `multidimio-0.7.3/src/mdio/segy/utilities.py` & `multidimio-0.7.4/src/mdio/segy/utilities.py`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,9 @@
 """More utilities for reading SEG-Ys."""
 
-
 from __future__ import annotations
 
 from typing import Sequence
 
 import numpy as np
 from dask.array.core import auto_chunks
 from numpy.typing import DTypeLike
```

### Comparing `multidimio-0.7.3/PKG-INFO` & `multidimio-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidimio
-Version: 0.7.3
+Version: 0.7.4
 Summary: Cloud-native, scalable, and user-friendly multi dimensional energy data!
 Home-page: https://mdio.dev
 License: Apache-2.0
 Keywords: mdio,multidimio,seismic,wind,data
 Author: TGS
 Author-email: sys-opensource@tgs.com
 Maintainer: Altay Sansal
```

