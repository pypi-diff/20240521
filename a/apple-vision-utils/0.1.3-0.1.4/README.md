# Comparing `tmp/apple_vision_utils-0.1.3.tar.gz` & `tmp/apple_vision_utils-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apple_vision_utils-0.1.3.tar", max compression
+gzip compressed data, was "apple_vision_utils-0.1.4.tar", max compression
```

## Comparing `apple_vision_utils-0.1.3.tar` & `apple_vision_utils-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2719 2024-05-21 17:35:14.686164 apple_vision_utils-0.1.3/README.md
--rw-r--r--   0        0        0       22 2024-05-21 17:35:24.483646 apple_vision_utils-0.1.3/apple_vision_utils/__init__.py
--rw-r--r--   0        0        0     4517 2024-05-21 17:18:09.479553 apple_vision_utils-0.1.3/apple_vision_utils/cli.py
--rw-r--r--   0        0        0      916 2024-05-21 17:35:24.483204 apple_vision_utils-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3766 1970-01-01 00:00:00.000000 apple_vision_utils-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2985 2024-05-21 17:40:12.162343 apple_vision_utils-0.1.4/README.md
+-rw-r--r--   0        0        0       22 2024-05-21 17:40:16.378824 apple_vision_utils-0.1.4/apple_vision_utils/__init__.py
+-rw-r--r--   0        0        0     4517 2024-05-21 17:18:09.479553 apple_vision_utils-0.1.4/apple_vision_utils/cli.py
+-rw-r--r--   0        0        0      916 2024-05-21 17:40:16.378346 apple_vision_utils-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4032 1970-01-01 00:00:00.000000 apple_vision_utils-0.1.4/PKG-INFO
```

### Comparing `apple_vision_utils-0.1.3/README.md` & `apple_vision_utils-0.1.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -24,14 +24,20 @@
 
 Below is the output of running the [tests](#test):
 
 https://g.teddysc.me/96d5b1217b90035c163b3c97ce99112f
 
 ## Installation
 
+Requires Python >= 3.11, <4.0.
+
+Since this package uses Apple's Vision framework, it only works on macOS.
+
+To OCR PDFs with `-p`, you need to install required dependency `poppler` with `brew install poppler` ([detailed guide](https://github.com/Belval/pdf2image)).
+
 ### pipx
 
 This is the recommended installation method.
 
 ```
 $ pipx install apple-vision-utils
 ```
```

### Comparing `apple_vision_utils-0.1.3/apple_vision_utils/cli.py` & `apple_vision_utils-0.1.4/apple_vision_utils/cli.py`

 * *Files identical despite different names*

### Comparing `apple_vision_utils-0.1.3/pyproject.toml` & `apple_vision_utils-0.1.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apple-vision-utils"
-version = "0.1.3"
+version = "0.1.4"
 description = "Fast and accurate OCR on images and PDFs using Apple Vision framework directly from command line."
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/tddschn/apple-vision-utils"
 repository = "https://github.com/tddschn/apple-vision-utils"
 classifiers = ["Topic :: Utilities"]
```

### Comparing `apple_vision_utils-0.1.3/PKG-INFO` & `apple_vision_utils-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apple-vision-utils
-Version: 0.1.3
+Version: 0.1.4
 Summary: Fast and accurate OCR on images and PDFs using Apple Vision framework directly from command line.
 Home-page: https://github.com/tddschn/apple-vision-utils
 License: MIT
 Keywords: ocr,apple-vision-framework
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
@@ -48,14 +48,20 @@
 
 Below is the output of running the [tests](#test):
 
 https://g.teddysc.me/96d5b1217b90035c163b3c97ce99112f
 
 ## Installation
 
+Requires Python >= 3.11, <4.0.
+
+Since this package uses Apple's Vision framework, it only works on macOS.
+
+To OCR PDFs with `-p`, you need to install required dependency `poppler` with `brew install poppler` ([detailed guide](https://github.com/Belval/pdf2image)).
+
 ### pipx
 
 This is the recommended installation method.
 
 ```
 $ pipx install apple-vision-utils
 ```
```

