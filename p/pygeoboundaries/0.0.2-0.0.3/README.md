# Comparing `tmp/pygeoboundaries-0.0.2.tar.gz` & `tmp/pygeoboundaries-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygeoboundaries-0.0.2.tar", max compression
+gzip compressed data, was "pygeoboundaries-0.0.3.tar", max compression
```

## Comparing `pygeoboundaries-0.0.2.tar` & `pygeoboundaries-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1055 2024-01-19 17:24:08.282710 pygeoboundaries-0.0.2/README.md
--rw-r--r--   0        0        0       53 2024-01-22 17:50:26.141216 pygeoboundaries-0.0.2/pygeoboundaries/__init__.py
--rw-r--r--   0        0        0    21449 2024-01-22 14:25:40.669151 pygeoboundaries-0.0.2/pygeoboundaries/pygeoboundaries.py
--rw-r--r--   0        0        0      705 2024-01-22 17:50:30.349249 pygeoboundaries-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1897 1970-01-01 00:00:00.000000 pygeoboundaries-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1055 2024-05-20 19:05:08.114344 pygeoboundaries-0.0.3/README.md
+-rw-r--r--   0        0        0       53 2024-05-20 19:05:08.114344 pygeoboundaries-0.0.3/pygeoboundaries/__init__.py
+-rw-r--r--   0        0        0    21449 2024-05-20 19:05:08.114344 pygeoboundaries-0.0.3/pygeoboundaries/pygeoboundaries.py
+-rw-r--r--   0        0        0      868 2024-05-20 19:05:08.114344 pygeoboundaries-0.0.3/pygeoboundaries/requirements.txt
+-rw-r--r--   0        0        0      705 2024-05-21 18:37:34.642279 pygeoboundaries-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1897 1970-01-01 00:00:00.000000 pygeoboundaries-0.0.3/PKG-INFO
```

### Comparing `pygeoboundaries-0.0.2/README.md` & `pygeoboundaries-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pygeoboundaries-0.0.2/pygeoboundaries/pygeoboundaries.py` & `pygeoboundaries-0.0.3/pygeoboundaries/pygeoboundaries.py`

 * *Files identical despite different names*

### Comparing `pygeoboundaries-0.0.2/pyproject.toml` & `pygeoboundaries-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygeoboundaries"
-version = "0.0.2"
+version = "0.0.3"
 description = "For performing data checks and file validation on geoboundary files. The primary purpose of this package is to facilitate the review process for pull requests made to the geoBoundaries repository."
 authors = ["rohith4444 <rohithreddy24242@gmail.com>", "DanRunfola <danr@wm.edu>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/wmgeolab/pyGeoBoundaries"
 repository = "https://github.com/wmgeolab/pyGeoBoundaries"
 keywords = ["pygeoboundaries","geoboundaries","wmgeolab","metaCheck"]
```

### Comparing `pygeoboundaries-0.0.2/PKG-INFO` & `pygeoboundaries-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeoboundaries
-Version: 0.0.2
+Version: 0.0.3
 Summary: For performing data checks and file validation on geoboundary files. The primary purpose of this package is to facilitate the review process for pull requests made to the geoBoundaries repository.
 Home-page: https://github.com/wmgeolab/pyGeoBoundaries
 License: MIT
 Keywords: pygeoboundaries,geoboundaries,wmgeolab,metaCheck
 Author: rohith4444
 Author-email: rohithreddy24242@gmail.com
 Requires-Python: >=3.9,<4.0
```

