# Comparing `tmp/data_source_local-0.0.4.tar.gz` & `tmp/data_source_local-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_source_local-0.0.4.tar", last modified: Mon May 20 21:58:59 2024, max compression
+gzip compressed data, was "data_source_local-0.0.5.tar", last modified: Tue May 21 06:34:46 2024, max compression
```

## Comparing `data_source_local-0.0.4.tar` & `data_source_local-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:58:59.087376 data_source_local-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-20 21:58:59.087376 data_source_local-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-20 21:58:36.000000 data_source_local-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:58:59.083376 data_source_local-0.0.4/data_source_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:58:59.087376 data_source_local-0.0.4/data_source_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 21:58:36.000000 data_source_local-0.0.4/data_source_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-20 21:58:36.000000 data_source_local-0.0.4/data_source_local/src/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-20 21:58:36.000000 data_source_local-0.0.4/data_source_local/src/data_source_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-20 21:58:36.000000 data_source_local-0.0.4/data_source_local/src/data_source_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:58:59.087376 data_source_local-0.0.4/data_source_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-20 21:58:59.000000 data_source_local-0.0.4/data_source_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-20 21:58:59.000000 data_source_local-0.0.4/data_source_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 21:58:59.000000 data_source_local-0.0.4/data_source_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-20 21:58:59.000000 data_source_local-0.0.4/data_source_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-20 21:58:59.000000 data_source_local-0.0.4/data_source_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-20 21:58:36.000000 data_source_local-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 21:58:59.087376 data_source_local-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-20 21:58:36.000000 data_source_local-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:34:46.471400 data_source_local-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-21 06:34:46.471400 data_source_local-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-21 06:34:26.000000 data_source_local-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:34:46.471400 data_source_local-0.0.5/data_source_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:34:46.471400 data_source_local-0.0.5/data_source_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 06:34:26.000000 data_source_local-0.0.5/data_source_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-05-21 06:34:26.000000 data_source_local-0.0.5/data_source_local/src/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-21 06:34:26.000000 data_source_local-0.0.5/data_source_local/src/data_source_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-21 06:34:26.000000 data_source_local-0.0.5/data_source_local/src/data_source_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:34:46.471400 data_source_local-0.0.5/data_source_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-21 06:34:46.000000 data_source_local-0.0.5/data_source_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-21 06:34:46.000000 data_source_local-0.0.5/data_source_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 06:34:46.000000 data_source_local-0.0.5/data_source_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-21 06:34:46.000000 data_source_local-0.0.5/data_source_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 06:34:46.000000 data_source_local-0.0.5/data_source_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-21 06:34:26.000000 data_source_local-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 06:34:46.471400 data_source_local-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-21 06:34:26.000000 data_source_local-0.0.5/setup.py
```

### Comparing `data_source_local-0.0.4/README.md` & `data_source_local-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `data_source_local-0.0.4/setup.py` & `data_source_local-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "data-source-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/data-source-local
-    version='0.0.4',
+    version='0.0.5',
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description=PACKAGE_NAME,
```

