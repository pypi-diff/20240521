# Comparing `tmp/aesthetic_predictor-0.1.1.tar.gz` & `tmp/aesthetic_predictor-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aesthetic_predictor-0.1.1.tar", max compression
+gzip compressed data, was "aesthetic_predictor-0.1.2.tar", max compression
```

## Comparing `aesthetic_predictor-0.1.1.tar` & `aesthetic_predictor-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      221 2023-03-12 15:41:52.780317 aesthetic_predictor-0.1.1/aesthetic_predictor/__init__.py
--rw-r--r--   0        0        0     2502 2023-03-12 15:41:57.985777 aesthetic_predictor-0.1.1/aesthetic_predictor/libs.py
--rw-r--r--   0        0        0      664 2023-03-12 15:42:06.066123 aesthetic_predictor-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      394 2023-03-12 15:36:16.375167 aesthetic_predictor-0.1.1/README.md
--rw-r--r--   0        0        0     1240 1970-01-01 00:00:00.000000 aesthetic_predictor-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      221 2024-05-21 12:32:03.054580 aesthetic_predictor-0.1.2/aesthetic_predictor/__init__.py
+-rw-r--r--   0        0        0     2502 2024-05-21 10:12:35.507449 aesthetic_predictor-0.1.2/aesthetic_predictor/libs.py
+-rw-r--r--   0        0        0      666 2024-05-21 12:32:08.683619 aesthetic_predictor-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1180 2024-05-21 10:12:35.507449 aesthetic_predictor-0.1.2/README.md
+-rw-r--r--   0        0        0     2025 1970-01-01 00:00:00.000000 aesthetic_predictor-0.1.2/PKG-INFO
```

### Comparing `aesthetic_predictor-0.1.1/aesthetic_predictor/libs.py` & `aesthetic_predictor-0.1.2/aesthetic_predictor/libs.py`

 * *Files identical despite different names*

