# Comparing `tmp/pynenv-0.1.0.tar.gz` & `tmp/pynenv-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynenv-0.1.0.tar", max compression
+gzip compressed data, was "pynenv-0.1.1.tar", max compression
```

## Comparing `pynenv-0.1.0.tar` & `pynenv-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       56 2024-05-21 06:04:41.890768 pynenv-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-20 20:07:32.307094 pynenv-0.1.0/pynenv/__init__.py
--rw-r--r--   0        0        0      542 2024-05-20 20:08:40.223334 pynenv-0.1.0/pynenv/environment.py
--rw-r--r--   0        0        0      267 2024-05-21 06:03:56.379064 pynenv-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      342 1970-01-01 00:00:00.000000 pynenv-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       56 2024-05-21 06:04:41.890768 pynenv-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 20:07:32.307094 pynenv-0.1.1/pynenv/__init__.py
+-rw-r--r--   0        0        0      542 2024-05-20 20:08:40.223334 pynenv-0.1.1/pynenv/environment.py
+-rw-r--r--   0        0        0      285 2024-05-21 06:15:42.841187 pynenv-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      381 1970-01-01 00:00:00.000000 pynenv-0.1.1/PKG-INFO
```

### Comparing `pynenv-0.1.0/pynenv/environment.py` & `pynenv-0.1.1/pynenv/environment.py`

 * *Files identical despite different names*

