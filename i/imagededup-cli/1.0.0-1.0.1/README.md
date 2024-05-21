# Comparing `tmp/imagededup-cli-1.0.0.tar.gz` & `tmp/imagededup-cli-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imagededup-cli-1.0.0.tar", last modified: Tue May 21 03:37:09 2024, max compression
+gzip compressed data, was "imagededup-cli-1.0.1.tar", last modified: Tue May 21 04:14:18 2024, max compression
```

## Comparing `imagededup-cli-1.0.0.tar` & `imagededup-cli-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-21 03:37:09.516429 imagededup-cli-1.0.0/
--rw-r--r--   0 tadeasfort   (501) staff       (20)        0 2024-05-21 02:18:29.000000 imagededup-cli-1.0.0/LICENSE
--rw-r--r--   0 tadeasfort   (501) staff       (20)      480 2024-05-21 03:37:09.516316 imagededup-cli-1.0.0/PKG-INFO
-drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-21 03:37:09.515489 imagededup-cli-1.0.0/imagededup_cli/
--rw-r--r--   0 tadeasfort   (501) staff       (20)        0 2024-05-21 02:18:11.000000 imagededup-cli-1.0.0/imagededup_cli/__init__.py
--rw-r--r--   0 tadeasfort   (501) staff       (20)     2857 2024-05-21 03:36:46.000000 imagededup-cli-1.0.0/imagededup_cli/imagededup_cli.py
-drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-21 03:37:09.516165 imagededup-cli-1.0.0/imagededup_cli.egg-info/
--rw-r--r--   0 tadeasfort   (501) staff       (20)      480 2024-05-21 03:37:09.000000 imagededup-cli-1.0.0/imagededup_cli.egg-info/PKG-INFO
--rw-r--r--   0 tadeasfort   (501) staff       (20)      306 2024-05-21 03:37:09.000000 imagededup-cli-1.0.0/imagededup_cli.egg-info/SOURCES.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)        1 2024-05-21 03:37:09.000000 imagededup-cli-1.0.0/imagededup_cli.egg-info/dependency_links.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)       70 2024-05-21 03:37:09.000000 imagededup-cli-1.0.0/imagededup_cli.egg-info/entry_points.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)       32 2024-05-21 03:37:09.000000 imagededup-cli-1.0.0/imagededup_cli.egg-info/requires.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)       15 2024-05-21 03:37:09.000000 imagededup-cli-1.0.0/imagededup_cli.egg-info/top_level.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)       38 2024-05-21 03:37:09.516467 imagededup-cli-1.0.0/setup.cfg
--rw-r--r--   0 tadeasfort   (501) staff       (20)      904 2024-05-21 03:34:46.000000 imagededup-cli-1.0.0/setup.py
+drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-21 04:14:18.576816 imagededup-cli-1.0.1/
+-rw-r--r--   0 tadeasfort   (501) staff       (20)        0 2024-05-21 02:18:29.000000 imagededup-cli-1.0.1/LICENSE
+-rw-r--r--   0 tadeasfort   (501) staff       (20)      480 2024-05-21 04:14:18.576679 imagededup-cli-1.0.1/PKG-INFO
+drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-21 04:14:18.575808 imagededup-cli-1.0.1/imagededup_cli/
+-rw-r--r--   0 tadeasfort   (501) staff       (20)        0 2024-05-21 02:18:11.000000 imagededup-cli-1.0.1/imagededup_cli/__init__.py
+-rw-r--r--   0 tadeasfort   (501) staff       (20)     4737 2024-05-21 04:13:11.000000 imagededup-cli-1.0.1/imagededup_cli/imagededup_cli.py
+drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-21 04:14:18.576503 imagededup-cli-1.0.1/imagededup_cli.egg-info/
+-rw-r--r--   0 tadeasfort   (501) staff       (20)      480 2024-05-21 04:14:18.000000 imagededup-cli-1.0.1/imagededup_cli.egg-info/PKG-INFO
+-rw-r--r--   0 tadeasfort   (501) staff       (20)      306 2024-05-21 04:14:18.000000 imagededup-cli-1.0.1/imagededup_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)        1 2024-05-21 04:14:18.000000 imagededup-cli-1.0.1/imagededup_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)       70 2024-05-21 04:14:18.000000 imagededup-cli-1.0.1/imagededup_cli.egg-info/entry_points.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)       32 2024-05-21 04:14:18.000000 imagededup-cli-1.0.1/imagededup_cli.egg-info/requires.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)       15 2024-05-21 04:14:18.000000 imagededup-cli-1.0.1/imagededup_cli.egg-info/top_level.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)       38 2024-05-21 04:14:18.576856 imagededup-cli-1.0.1/setup.cfg
+-rw-r--r--   0 tadeasfort   (501) staff       (20)      904 2024-05-21 04:13:57.000000 imagededup-cli-1.0.1/setup.py
```

### Comparing `imagededup-cli-1.0.0/setup.py` & `imagededup-cli-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="imagededup-cli",  # Package name
-    version="1.0.0",  # Initial version
+    version="1.0.1",  # Initial version
     author="Tadeas Fort",
     author_email="taddy.fort@gmail.com",
     description="A tool to remove duplicate jpg images",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/tadeasf/imagededup-cli",  # Project URL
     packages=find_packages(),
```

