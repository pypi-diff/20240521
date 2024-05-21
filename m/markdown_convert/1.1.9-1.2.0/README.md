# Comparing `tmp/markdown_convert-1.1.9.tar.gz` & `tmp/markdown_convert-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_convert-1.1.9.tar", max compression
+gzip compressed data, was "markdown_convert-1.2.0.tar", max compression
```

## Comparing `markdown_convert-1.1.9.tar` & `markdown_convert-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    18092 2023-10-23 17:37:06.761873 markdown_convert-1.1.9/LICENSE
--rw-r--r--   0        0        0     2452 2024-04-18 14:09:49.066892 markdown_convert-1.1.9/README.md
--rw-r--r--   0        0        0      213 2024-04-10 10:59:42.869680 markdown_convert-1.1.9/markdown_convert/__init__.py
--rwxr-xr-x   0        0        0     2815 2024-04-09 12:12:31.637276 markdown_convert-1.1.9/markdown_convert/__main__.py
--rw-r--r--   0        0        0     4935 2024-04-08 12:12:18.468503 markdown_convert-1.1.9/markdown_convert/code.css
--rw-r--r--   0        0        0     5680 2024-05-20 09:30:39.806398 markdown_convert-1.1.9/markdown_convert/default.css
--rw-r--r--   0        0        0       65 2024-04-10 10:59:51.693837 markdown_convert-1.1.9/markdown_convert/modules/__init__.py
--rw-r--r--   0        0        0      429 2024-04-10 20:54:32.247070 markdown_convert-1.1.9/markdown_convert/modules/constants.py
--rw-r--r--   0        0        0     5711 2024-04-16 12:03:21.481233 markdown_convert-1.1.9/markdown_convert/modules/convert.py
--rw-r--r--   0        0        0     2258 2024-04-09 12:12:32.309271 markdown_convert-1.1.9/markdown_convert/modules/resources.py
--rw-r--r--   0        0        0      655 2024-04-10 10:56:40.081145 markdown_convert-1.1.9/markdown_convert/modules/utils.py
--rw-r--r--   0        0        0     1487 2024-04-08 14:48:42.000577 markdown_convert-1.1.9/markdown_convert/modules/validate.py
--rw-r--r--   0        0        0      680 2024-05-20 10:11:09.842565 markdown_convert-1.1.9/pyproject.toml
--rw-r--r--   0        0        0     3356 1970-01-01 00:00:00.000000 markdown_convert-1.1.9/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-10-23 17:37:06.761873 markdown_convert-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2452 2024-04-18 14:09:49.066892 markdown_convert-1.2.0/README.md
+-rw-r--r--   0        0        0      213 2024-04-10 10:59:42.869680 markdown_convert-1.2.0/markdown_convert/__init__.py
+-rwxr-xr-x   0        0        0     2815 2024-04-09 12:12:31.637276 markdown_convert-1.2.0/markdown_convert/__main__.py
+-rw-r--r--   0        0        0     4935 2024-04-08 12:12:18.468503 markdown_convert-1.2.0/markdown_convert/code.css
+-rw-r--r--   0        0        0     5680 2024-05-20 09:30:39.806398 markdown_convert-1.2.0/markdown_convert/default.css
+-rw-r--r--   0        0        0       65 2024-04-10 10:59:51.693837 markdown_convert-1.2.0/markdown_convert/modules/__init__.py
+-rw-r--r--   0        0        0      429 2024-04-10 20:54:32.247070 markdown_convert-1.2.0/markdown_convert/modules/constants.py
+-rw-r--r--   0        0        0     5711 2024-04-16 12:03:21.481233 markdown_convert-1.2.0/markdown_convert/modules/convert.py
+-rw-r--r--   0        0        0     2258 2024-04-09 12:12:32.309271 markdown_convert-1.2.0/markdown_convert/modules/resources.py
+-rw-r--r--   0        0        0      655 2024-04-10 10:56:40.081145 markdown_convert-1.2.0/markdown_convert/modules/utils.py
+-rw-r--r--   0        0        0     1487 2024-04-08 14:48:42.000577 markdown_convert-1.2.0/markdown_convert/modules/validate.py
+-rw-r--r--   0        0        0      717 2024-05-21 07:50:02.421195 markdown_convert-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3266 1970-01-01 00:00:00.000000 markdown_convert-1.2.0/PKG-INFO
```

### Comparing `markdown_convert-1.1.9/LICENSE` & `markdown_convert-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.1.9/README.md` & `markdown_convert-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.1.9/markdown_convert/__main__.py` & `markdown_convert-1.2.0/markdown_convert/__main__.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.1.9/markdown_convert/code.css` & `markdown_convert-1.2.0/markdown_convert/code.css`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.1.9/markdown_convert/default.css` & `markdown_convert-1.2.0/markdown_convert/default.css`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.1.9/markdown_convert/modules/convert.py` & `markdown_convert-1.2.0/markdown_convert/modules/convert.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.1.9/markdown_convert/modules/resources.py` & `markdown_convert-1.2.0/markdown_convert/modules/resources.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.1.9/markdown_convert/modules/utils.py` & `markdown_convert-1.2.0/markdown_convert/modules/utils.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.1.9/markdown_convert/modules/validate.py` & `markdown_convert-1.2.0/markdown_convert/modules/validate.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.1.9/pyproject.toml` & `markdown_convert-1.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "markdown_convert"
-version = "1.1.9"
+version = "1.2.0"
 description = "Convert Markdown files to PDF from your command line."
 authors = ["Julio Cabria <juliocabria@tutanota.com>"]
 license = "GPL-2.0-only"
 readme = "README.md"
 homepage = "https://github.com/Julynx/markdown_convert"
 include = ["markdown_convert/default.css", "markdown_convert/code.css"]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
+python = ">=3.10,<4.0"
 argsdict = "1.0.0"
-setuptools = ">=46.0.0"
-weasyprint = "^61.2"
-markdown2 = "^2.4.13"
-pygments = "^2.17.2"
+setuptools = ">=46.0.0, <100.0.0"
+weasyprint = ">=62.1, <70.0"
+markdown2 = ">=2.4.13, <3.0.0"
+pygments = ">=2.17.2, <3.0.0"
 
 [tool.poetry.scripts]
 markdown-convert = "markdown_convert.__main__:main"
```

### Comparing `markdown_convert-1.1.9/PKG-INFO` & `markdown_convert-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: markdown_convert
-Version: 1.1.9
+Version: 1.2.0
 Summary: Convert Markdown files to PDF from your command line.
 Home-page: https://github.com/Julynx/markdown_convert
 License: GPL-2.0-only
 Author: Julio Cabria
 Author-email: juliocabria@tutanota.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: argsdict (==1.0.0)
 Requires-Dist: markdown2 (>=2.4.13,<3.0.0)
 Requires-Dist: pygments (>=2.17.2,<3.0.0)
-Requires-Dist: setuptools (>=46.0.0)
-Requires-Dist: weasyprint (>=61.2,<62.0)
+Requires-Dist: setuptools (>=46.0.0,<100.0.0)
+Requires-Dist: weasyprint (>=62.1,<70.0)
 Description-Content-Type: text/markdown
 
 # markdown-convert
 
 _Convert Markdown files to PDF from your command line._
 
 ### `pip install markdown-convert`
```

