# Comparing `tmp/apple_vision_utils-0.1.2.tar.gz` & `tmp/apple_vision_utils-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apple_vision_utils-0.1.2.tar", max compression
+gzip compressed data, was "apple_vision_utils-0.1.3.tar", max compression
```

## Comparing `apple_vision_utils-0.1.2.tar` & `apple_vision_utils-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2663 2024-05-21 17:32:43.150755 apple_vision_utils-0.1.2/README.md
--rw-r--r--   0        0        0       22 2024-05-21 17:33:01.059570 apple_vision_utils-0.1.2/apple_vision_utils/__init__.py
--rw-r--r--   0        0        0     4517 2024-05-21 17:18:09.479553 apple_vision_utils-0.1.2/apple_vision_utils/cli.py
--rw-r--r--   0        0        0      916 2024-05-21 17:33:01.058838 apple_vision_utils-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3710 1970-01-01 00:00:00.000000 apple_vision_utils-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2719 2024-05-21 17:35:14.686164 apple_vision_utils-0.1.3/README.md
+-rw-r--r--   0        0        0       22 2024-05-21 17:35:24.483646 apple_vision_utils-0.1.3/apple_vision_utils/__init__.py
+-rw-r--r--   0        0        0     4517 2024-05-21 17:18:09.479553 apple_vision_utils-0.1.3/apple_vision_utils/cli.py
+-rw-r--r--   0        0        0      916 2024-05-21 17:35:24.483204 apple_vision_utils-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3766 1970-01-01 00:00:00.000000 apple_vision_utils-0.1.3/PKG-INFO
```

### Comparing `apple_vision_utils-0.1.2/README.md` & `apple_vision_utils-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # Apple Vision Framework Python Utilities
 
-Fast and accurate OCR on images and PDFs using Apple Vision framework directly from command line.
+Fast and accurate OCR on images and PDFs using Apple Vision framework (`pyobjc-framework-Vision`) directly from command line.
 
 - [Apple Vision Framework Python Utilities](#apple-vision-framework-python-utilities)
   - [Features](#features)
   - [Demo](#demo)
   - [Installation](#installation)
     - [pipx](#pipx)
     - [pip](#pip)
   - [Usage](#usage)
   - [Develop](#develop)
   - [Test](#test)
 
 ## Features
 
-- Fast and accurate, multi-language support (`-l`, `--lang`), powered by Apple's industry-strength Vision framework.
+- Fast and accurate, multi-language support (`-l`, `--lang`), powered by Apple's industry-strength Vision framework (`pyobjc-framework-Vision`).
 - Supports all common input image formats: PNG, JPEG, TIFF and WebP.
 - Supports PDF input (the file gets converted to images first). This tool does NOT assume a file is PDF just because it has a `.pdf` extension, you need to pass `-p`, `--pdf` flag.
 - Outputs extracted text only by default, but can output in JSON format containing confidence of recognition for each line with `-j`, `--json` flag.
 
 
 ## Demo
```

### Comparing `apple_vision_utils-0.1.2/apple_vision_utils/cli.py` & `apple_vision_utils-0.1.3/apple_vision_utils/cli.py`

 * *Files identical despite different names*

### Comparing `apple_vision_utils-0.1.2/pyproject.toml` & `apple_vision_utils-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apple-vision-utils"
-version = "0.1.2"
+version = "0.1.3"
 description = "Fast and accurate OCR on images and PDFs using Apple Vision framework directly from command line."
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/tddschn/apple-vision-utils"
 repository = "https://github.com/tddschn/apple-vision-utils"
 classifiers = ["Topic :: Utilities"]
```

### Comparing `apple_vision_utils-0.1.2/PKG-INFO` & `apple_vision_utils-0.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apple-vision-utils
-Version: 0.1.2
+Version: 0.1.3
 Summary: Fast and accurate OCR on images and PDFs using Apple Vision framework directly from command line.
 Home-page: https://github.com/tddschn/apple-vision-utils
 License: MIT
 Keywords: ocr,apple-vision-framework
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
@@ -20,29 +20,29 @@
 Requires-Dist: wurlitzer (>=3.1.0,<4.0.0)
 Project-URL: Bug Tracker, https://github.com/tddschn/apple-vision-utils/issues
 Project-URL: Repository, https://github.com/tddschn/apple-vision-utils
 Description-Content-Type: text/markdown
 
 # Apple Vision Framework Python Utilities
 
-Fast and accurate OCR on images and PDFs using Apple Vision framework directly from command line.
+Fast and accurate OCR on images and PDFs using Apple Vision framework (`pyobjc-framework-Vision`) directly from command line.
 
 - [Apple Vision Framework Python Utilities](#apple-vision-framework-python-utilities)
   - [Features](#features)
   - [Demo](#demo)
   - [Installation](#installation)
     - [pipx](#pipx)
     - [pip](#pip)
   - [Usage](#usage)
   - [Develop](#develop)
   - [Test](#test)
 
 ## Features
 
-- Fast and accurate, multi-language support (`-l`, `--lang`), powered by Apple's industry-strength Vision framework.
+- Fast and accurate, multi-language support (`-l`, `--lang`), powered by Apple's industry-strength Vision framework (`pyobjc-framework-Vision`).
 - Supports all common input image formats: PNG, JPEG, TIFF and WebP.
 - Supports PDF input (the file gets converted to images first). This tool does NOT assume a file is PDF just because it has a `.pdf` extension, you need to pass `-p`, `--pdf` flag.
 - Outputs extracted text only by default, but can output in JSON format containing confidence of recognition for each line with `-j`, `--json` flag.
 
 
 ## Demo
```

