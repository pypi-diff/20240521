# Comparing `tmp/apple_vision_utils-0.1.1.tar.gz` & `tmp/apple_vision_utils-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apple_vision_utils-0.1.1.tar", max compression
+gzip compressed data, was "apple_vision_utils-0.1.2.tar", max compression
```

## Comparing `apple_vision_utils-0.1.1.tar` & `apple_vision_utils-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-05-21 16:58:19.754302 apple_vision_utils-0.1.1/README.md
--rw-r--r--   0        0        0       22 2024-05-21 17:18:20.109120 apple_vision_utils-0.1.1/apple_vision_utils/__init__.py
--rw-r--r--   0        0        0     4517 2024-05-21 17:18:09.479553 apple_vision_utils-0.1.1/apple_vision_utils/cli.py
--rw-r--r--   0        0        0      916 2024-05-21 17:18:20.108407 apple_vision_utils-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1047 1970-01-01 00:00:00.000000 apple_vision_utils-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2663 2024-05-21 17:32:43.150755 apple_vision_utils-0.1.2/README.md
+-rw-r--r--   0        0        0       22 2024-05-21 17:33:01.059570 apple_vision_utils-0.1.2/apple_vision_utils/__init__.py
+-rw-r--r--   0        0        0     4517 2024-05-21 17:18:09.479553 apple_vision_utils-0.1.2/apple_vision_utils/cli.py
+-rw-r--r--   0        0        0      916 2024-05-21 17:33:01.058838 apple_vision_utils-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3710 1970-01-01 00:00:00.000000 apple_vision_utils-0.1.2/PKG-INFO
```

### Comparing `apple_vision_utils-0.1.1/apple_vision_utils/cli.py` & `apple_vision_utils-0.1.2/apple_vision_utils/cli.py`

 * *Files identical despite different names*

### Comparing `apple_vision_utils-0.1.1/pyproject.toml` & `apple_vision_utils-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apple-vision-utils"
-version = "0.1.1"
+version = "0.1.2"
 description = "Fast and accurate OCR on images and PDFs using Apple Vision framework directly from command line."
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/tddschn/apple-vision-utils"
 repository = "https://github.com/tddschn/apple-vision-utils"
 classifiers = ["Topic :: Utilities"]
```

