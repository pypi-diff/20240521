# Comparing `tmp/starbear-0.1.4.tar.gz` & `tmp/starbear-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starbear-0.1.4.tar", max compression
+gzip compressed data, was "starbear-0.1.5.tar", max compression
```

## Comparing `starbear-0.1.4.tar` & `starbear-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      708 2024-05-17 18:53:54.379104 starbear-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      383 2024-05-02 20:10:45.559615 starbear-0.1.4/starbear/__init__.py
--rw-r--r--   0        0        0      276 2023-12-18 19:59:00.300414 starbear-0.1.4/starbear/bearlib-template.html
--rw-r--r--   0        0        0    23883 2024-04-26 19:04:39.586276 starbear-0.1.4/starbear/bearlib.js
--rw-r--r--   0        0        0     1049 2024-02-02 19:46:01.148155 starbear-0.1.4/starbear/bearstyle.css
--rw-r--r--   0        0        0     2206 2024-02-29 00:50:48.026310 starbear-0.1.4/starbear/constructors.py
--rw-r--r--   0        0        0      322 2024-02-12 21:08:30.565978 starbear-0.1.4/starbear/page-template.html
--rw-r--r--   0        0        0    10370 2024-05-02 20:12:38.546585 starbear-0.1.4/starbear/page.py
--rw-r--r--   0        0        0     2226 2024-05-02 20:12:38.548759 starbear-0.1.4/starbear/ref.py
--rw-r--r--   0        0        0     7708 2024-02-01 21:14:06.522289 starbear-0.1.4/starbear/repr.py
--rw-r--r--   0        0        0    19006 2024-05-02 20:22:05.098297 starbear-0.1.4/starbear/serve.py
--rw-r--r--   0        0        0     4117 2024-01-19 16:02:41.325613 starbear-0.1.4/starbear/templating.py
--rw-r--r--   0        0        0     4831 2024-05-17 18:44:07.443188 starbear-0.1.4/starbear/utils.py
--rw-r--r--   0        0        0       18 2024-05-17 18:53:54.400658 starbear-0.1.4/starbear/version.py
--rw-r--r--   0        0        0      700 1970-01-01 00:00:00.000000 starbear-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      708 2024-05-21 18:12:31.373499 starbear-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      383 2024-05-02 20:10:45.559615 starbear-0.1.5/starbear/__init__.py
+-rw-r--r--   0        0        0      276 2023-12-18 19:59:00.300414 starbear-0.1.5/starbear/bearlib-template.html
+-rw-r--r--   0        0        0    23883 2024-04-26 19:04:39.586276 starbear-0.1.5/starbear/bearlib.js
+-rw-r--r--   0        0        0     1049 2024-02-02 19:46:01.148155 starbear-0.1.5/starbear/bearstyle.css
+-rw-r--r--   0        0        0     2206 2024-02-29 00:50:48.026310 starbear-0.1.5/starbear/constructors.py
+-rw-r--r--   0        0        0      322 2024-02-12 21:08:30.565978 starbear-0.1.5/starbear/page-template.html
+-rw-r--r--   0        0        0    10370 2024-05-02 20:12:38.546585 starbear-0.1.5/starbear/page.py
+-rw-r--r--   0        0        0     2226 2024-05-02 20:12:38.548759 starbear-0.1.5/starbear/ref.py
+-rw-r--r--   0        0        0     7708 2024-02-01 21:14:06.522289 starbear-0.1.5/starbear/repr.py
+-rw-r--r--   0        0        0    18990 2024-05-21 18:11:04.905711 starbear-0.1.5/starbear/serve.py
+-rw-r--r--   0        0        0     4117 2024-01-19 16:02:41.325613 starbear-0.1.5/starbear/templating.py
+-rw-r--r--   0        0        0     4797 2024-05-21 18:11:18.304014 starbear-0.1.5/starbear/utils.py
+-rw-r--r--   0        0        0       18 2024-05-21 18:12:31.402103 starbear-0.1.5/starbear/version.py
+-rw-r--r--   0        0        0      700 1970-01-01 00:00:00.000000 starbear-0.1.5/PKG-INFO
```

### Comparing `starbear-0.1.4/pyproject.toml` & `starbear-0.1.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "starbear"
-version = "0.1.4"
+version = "0.1.5"
 description = "Framework for easy small local web apps or programs"
 authors = ["Olivier Breuleux <breuleux@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 uvicorn = ">=0.17.6"
```

### Comparing `starbear-0.1.4/starbear/bearlib.js` & `starbear-0.1.5/starbear/bearlib.js`

 * *Files identical despite different names*

### Comparing `starbear-0.1.4/starbear/bearstyle.css` & `starbear-0.1.5/starbear/bearstyle.css`

 * *Files identical despite different names*

### Comparing `starbear-0.1.4/starbear/constructors.py` & `starbear-0.1.5/starbear/constructors.py`

 * *Files identical despite different names*

### Comparing `starbear-0.1.4/starbear/page.py` & `starbear-0.1.5/starbear/page.py`

 * *Files identical despite different names*

### Comparing `starbear-0.1.4/starbear/ref.py` & `starbear-0.1.5/starbear/ref.py`

 * *Files identical despite different names*

### Comparing `starbear-0.1.4/starbear/repr.py` & `starbear-0.1.5/starbear/repr.py`

 * *Files identical despite different names*

### Comparing `starbear-0.1.4/starbear/serve.py` & `starbear-0.1.5/starbear/serve.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 import base64
 import inspect
 import json
 import os
 import traceback
 from contextvars import ContextVar
 from functools import cached_property, wraps
-from itertools import count
+from itertools import count, islice
 from pathlib import Path
 from uuid import uuid4 as uuid
 
 from hrepr import H, Tag
-from more_itertools import take
 from starlette.exceptions import HTTPException
 from starlette.responses import (
     FileResponse,
     HTMLResponse,
     JSONResponse,
     PlainTextResponse,
     RedirectResponse,
@@ -494,15 +493,15 @@
 
     #############
     # Utilities #
     #############
 
     def _create_new_cub(self, proc, query_params, session):
         reclaims = max(0, min(len(self.dormant_cubs), len(self.cubs) - self.soft_process_cap))
-        processes = take(n=reclaims, iterable=self.dormant_cubs)
+        processes = list(islice(n=reclaims, iterable=self.dormant_cubs))
 
         for p in processes:
             cub = self.dormant_cubs.pop(p)
             cub.destroy()
             del self.cubs[p]
 
         if len(self.cubs) > self.hard_process_cap:
```

### Comparing `starbear-0.1.4/starbear/templating.py` & `starbear-0.1.5/starbear/templating.py`

 * *Files identical despite different names*

### Comparing `starbear-0.1.4/starbear/utils.py` & `starbear-0.1.5/starbear/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import asyncio
 import functools
 import logging
 import sys
 import traceback
-from dataclasses import dataclass
 from hashlib import md5
 from mimetypes import guess_type
 
 from hrepr.resource import JSExpression
 
 from .ref import Reference
```

### Comparing `starbear-0.1.4/PKG-INFO` & `starbear-0.1.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starbear
-Version: 0.1.4
+Version: 0.1.5
 Summary: Framework for easy small local web apps or programs
 License: MIT
 Author: Olivier Breuleux
 Author-email: breuleux@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

