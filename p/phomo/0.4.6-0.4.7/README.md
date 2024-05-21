# Comparing `tmp/phomo-0.4.6.tar.gz` & `tmp/phomo-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phomo-0.4.6.tar", max compression
+gzip compressed data, was "phomo-0.4.7.tar", max compression
```

## Comparing `phomo-0.4.6.tar` & `phomo-0.4.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1068 2024-04-03 16:51:34.142816 phomo-0.4.6/LICENSE
--rw-r--r--   0        0        0     3948 2023-09-22 23:13:23.476798 phomo-0.4.6/README.md
--rw-r--r--   0        0        0      252 2023-09-22 23:13:23.476798 phomo-0.4.6/phomo/__init__.py
--rw-r--r--   0        0        0     4836 2022-01-14 16:40:00.300031 phomo-0.4.6/phomo/__main__.py
--rw-r--r--   0        0        0     6357 2023-09-22 22:30:39.853453 phomo-0.4.6/phomo/grid.py
--rw-r--r--   0        0        0     2631 2023-09-22 23:13:23.473465 phomo-0.4.6/phomo/master.py
--rw-r--r--   0        0        0     3465 2023-09-22 23:13:23.473465 phomo-0.4.6/phomo/metrics.py
--rw-r--r--   0        0        0    10980 2023-09-22 23:13:23.476798 phomo-0.4.6/phomo/mosaic.py
--rw-r--r--   0        0        0     2006 2023-09-22 23:13:23.476798 phomo-0.4.6/phomo/palette.py
--rw-r--r--   0        0        0     4233 2023-09-22 23:13:23.476798 phomo-0.4.6/phomo/pool.py
--rw-r--r--   0        0        0     4059 2023-09-22 23:13:23.476798 phomo-0.4.6/phomo/utils.py
--rw-r--r--   0        0        0     1043 2024-05-06 20:58:59.753747 phomo-0.4.6/pyproject.toml
--rw-r--r--   0        0        0     5231 1970-01-01 00:00:00.000000 phomo-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-03 16:51:34.142816 phomo-0.4.7/LICENSE
+-rw-r--r--   0        0        0     3948 2023-09-22 23:13:23.476798 phomo-0.4.7/README.md
+-rw-r--r--   0        0        0      252 2023-09-22 23:13:23.476798 phomo-0.4.7/phomo/__init__.py
+-rw-r--r--   0        0        0     4836 2022-01-14 16:40:00.300031 phomo-0.4.7/phomo/__main__.py
+-rw-r--r--   0        0        0     6357 2023-09-22 22:30:39.853453 phomo-0.4.7/phomo/grid.py
+-rw-r--r--   0        0        0     2631 2024-05-17 00:32:49.971993 phomo-0.4.7/phomo/master.py
+-rw-r--r--   0        0        0     3465 2023-09-22 23:13:23.473465 phomo-0.4.7/phomo/metrics.py
+-rw-r--r--   0        0        0    10980 2023-09-22 23:13:23.476798 phomo-0.4.7/phomo/mosaic.py
+-rw-r--r--   0        0        0     2006 2023-09-22 23:13:23.476798 phomo-0.4.7/phomo/palette.py
+-rw-r--r--   0        0        0     4233 2023-09-22 23:13:23.476798 phomo-0.4.7/phomo/pool.py
+-rw-r--r--   0        0        0     4059 2023-09-22 23:13:23.476798 phomo-0.4.7/phomo/utils.py
+-rw-r--r--   0        0        0     1029 2024-05-21 10:31:27.186675 phomo-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0     5231 1970-01-01 00:00:00.000000 phomo-0.4.7/PKG-INFO
```

### Comparing `phomo-0.4.6/LICENSE` & `phomo-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `phomo-0.4.6/README.md` & `phomo-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `phomo-0.4.6/phomo/__main__.py` & `phomo-0.4.7/phomo/__main__.py`

 * *Files identical despite different names*

### Comparing `phomo-0.4.6/phomo/grid.py` & `phomo-0.4.7/phomo/grid.py`

 * *Files identical despite different names*

### Comparing `phomo-0.4.6/phomo/master.py` & `phomo-0.4.7/phomo/master.py`

 * *Files identical despite different names*

### Comparing `phomo-0.4.6/phomo/metrics.py` & `phomo-0.4.7/phomo/metrics.py`

 * *Files identical despite different names*

### Comparing `phomo-0.4.6/phomo/mosaic.py` & `phomo-0.4.7/phomo/mosaic.py`

 * *Files identical despite different names*

### Comparing `phomo-0.4.6/phomo/palette.py` & `phomo-0.4.7/phomo/palette.py`

 * *Files identical despite different names*

### Comparing `phomo-0.4.6/phomo/pool.py` & `phomo-0.4.7/phomo/pool.py`

 * *Files identical despite different names*

### Comparing `phomo-0.4.6/phomo/utils.py` & `phomo-0.4.7/phomo/utils.py`

 * *Files identical despite different names*

### Comparing `phomo-0.4.6/pyproject.toml` & `phomo-0.4.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "phomo"
-version = "0.4.6"
+version = "0.4.7"
 description = "Python package and CLI utility to create photo mosaics."
 authors = ["Loic Coyle <loic.coyle@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/loiccoyle/phomo"
 keywords = ["photomosaic", "photographic", "mosaic", "art", "image"]
 classifiers = [
-    "Topic :: Software Development :: Libraries :: Python Modules",
-    "Programming Language :: Python :: 3 :: Only",
-    "Topic :: Scientific/Engineering :: Image Processing",
-    "Topic :: Artistic Software",
-    "Operating System :: MacOS",
-    "Operating System :: Microsoft :: Windows",
-    "Operating System :: POSIX :: Linux",
+  "Topic :: Software Development :: Libraries :: Python Modules",
+  "Programming Language :: Python :: 3 :: Only",
+  "Topic :: Scientific/Engineering :: Image Processing",
+  "Topic :: Artistic Software",
+  "Operating System :: MacOS",
+  "Operating System :: Microsoft :: Windows",
+  "Operating System :: POSIX :: Linux",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 pillow = "^10.0.1"
 numpy = "^1.22.0"
 tqdm = "^4.60.0"
```

### Comparing `phomo-0.4.6/PKG-INFO` & `phomo-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phomo
-Version: 0.4.6
+Version: 0.4.7
 Summary: Python package and CLI utility to create photo mosaics.
 Home-page: https://github.com/loiccoyle/phomo
 License: MIT
 Keywords: photomosaic,photographic,mosaic,art,image
 Author: Loic Coyle
 Author-email: loic.coyle@hotmail.fr
 Requires-Python: >=3.9,<3.13
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: phomo Version: 0.4.6 Summary: Python package and
+Metadata-Version: 2.1 Name: phomo Version: 0.4.7 Summary: Python package and
 CLI utility to create photo mosaics. Home-page: https://github.com/loiccoyle/
 phomo License: MIT Keywords: photomosaic,photographic,mosaic,art,image Author:
 Loic Coyle Author-email: loic.coyle@hotmail.fr Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: MacOS Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: POSIX :: Linux Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```

