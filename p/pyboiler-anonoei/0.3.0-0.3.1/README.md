# Comparing `tmp/pyboiler_anonoei-0.3.0.tar.gz` & `tmp/pyboiler_anonoei-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyboiler_anonoei-0.3.0.tar", last modified: Sun May 19 23:33:27 2024, max compression
+gzip compressed data, was "pyboiler_anonoei-0.3.1.tar", last modified: Tue May 21 06:34:45 2024, max compression
```

## Comparing `pyboiler_anonoei-0.3.0.tar` & `pyboiler_anonoei-0.3.1.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-19 23:33:27.479337 pyboiler_anonoei-0.3.0/
--rwxrwx---   0 anonoei    (501) staff       (20)     1051 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.3.0/LICENSE
--rw-r--r--   0 anonoei    (501) staff       (20)     1355 2024-05-19 23:33:27.478987 pyboiler_anonoei-0.3.0/PKG-INFO
--rwxrwx---   0 anonoei    (501) staff       (20)      281 2024-05-12 13:44:40.000000 pyboiler_anonoei-0.3.0/README.md
--rwxrwx---   0 anonoei    (501) staff       (20)     1423 2024-05-19 23:33:22.000000 pyboiler_anonoei-0.3.0/pyproject.toml
--rw-r--r--   0 anonoei    (501) staff       (20)       38 2024-05-19 23:33:27.479397 pyboiler_anonoei-0.3.0/setup.cfg
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-19 23:33:27.468031 pyboiler_anonoei-0.3.0/src/
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-19 23:33:27.473396 pyboiler_anonoei-0.3.0/src/pyboiler/
--rwxrwx---   0 anonoei    (501) staff       (20)      813 2024-05-19 23:31:32.000000 pyboiler_anonoei-0.3.0/src/pyboiler/__init__.py
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-19 23:33:27.473630 pyboiler_anonoei-0.3.0/src/pyboiler/_internal/
--rwxrwx---   0 anonoei    (501) staff       (20)        0 2024-05-17 22:45:41.000000 pyboiler_anonoei-0.3.0/src/pyboiler/_internal/__init__.py
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-19 23:33:27.474548 pyboiler_anonoei-0.3.0/src/pyboiler/_internal/color/
--rwxrwx---   0 anonoei    (501) staff       (20)       48 2024-05-18 00:12:37.000000 pyboiler_anonoei-0.3.0/src/pyboiler/_internal/color/__init__.py
--rwxrwx---   0 anonoei    (501) staff       (20)     2474 2024-05-19 22:15:06.000000 pyboiler_anonoei-0.3.0/src/pyboiler/_internal/color/colors.py
--rw-r--r--   0 anonoei    (501) staff       (20)      272 2024-05-19 21:50:23.000000 pyboiler_anonoei-0.3.0/src/pyboiler/_internal/color/config.py
--rwxrwx---   0 anonoei    (501) staff       (20)     1032 2024-05-19 21:38:25.000000 pyboiler_anonoei-0.3.0/src/pyboiler/_internal/color/parse.py
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-19 23:33:27.476437 pyboiler_anonoei-0.3.0/src/pyboiler/_internal/log/
--rwxrwx---   0 anonoei    (501) staff       (20)      256 2024-05-18 09:15:43.000000 pyboiler_anonoei-0.3.0/src/pyboiler/_internal/log/__init__.py
--rwxrwx---   0 anonoei    (501) staff       (20)      416 2024-05-19 22:46:14.000000 pyboiler_anonoei-0.3.0/src/pyboiler/_internal/log/config.py
--rwxrwx---   0 anonoei    (501) staff       (20)      478 2024-05-18 02:02:44.000000 pyboiler_anonoei-0.3.0/src/pyboiler/_internal/log/filter.py
--rwxrwx---   0 anonoei    (501) staff       (20)     3836 2024-05-19 22:17:46.000000 pyboiler_anonoei-0.3.0/src/pyboiler/_internal/log/format.py
--rwxrwx---   0 anonoei    (501) staff       (20)     2959 2024-05-19 23:10:46.000000 pyboiler_anonoei-0.3.0/src/pyboiler/_internal/log/handler.py
--rwxrwx---   0 anonoei    (501) staff       (20)      610 2024-05-19 19:07:04.000000 pyboiler_anonoei-0.3.0/src/pyboiler/_internal/log/inspect.py
--rwxrwx---   0 anonoei    (501) staff       (20)     1200 2024-05-19 21:55:02.000000 pyboiler_anonoei-0.3.0/src/pyboiler/_internal/log/level.py
--rwxrwx---   0 anonoei    (501) staff       (20)      517 2024-05-18 09:40:31.000000 pyboiler_anonoei-0.3.0/src/pyboiler/_internal/log/record.py
--rwxrwx---   0 anonoei    (501) staff       (20)     1331 2024-05-12 23:15:42.000000 pyboiler_anonoei-0.3.0/src/pyboiler/changelog.py
--rwxrwx---   0 anonoei    (501) staff       (20)       74 2024-05-18 00:12:59.000000 pyboiler_anonoei-0.3.0/src/pyboiler/color.py
--rwxrwx---   0 anonoei    (501) staff       (20)     2313 2024-05-12 10:43:02.000000 pyboiler_anonoei-0.3.0/src/pyboiler/config.py
--rwxrwx---   0 anonoei    (501) staff       (20)     1041 2024-05-17 18:25:19.000000 pyboiler_anonoei-0.3.0/src/pyboiler/decor.py
--rwxrwx---   0 anonoei    (501) staff       (20)      660 2024-05-12 23:46:14.000000 pyboiler_anonoei-0.3.0/src/pyboiler/error.py
--rwxrwx---   0 anonoei    (501) staff       (20)     4227 2024-05-19 23:26:23.000000 pyboiler_anonoei-0.3.0/src/pyboiler/generic.py
--rwxrwx---   0 anonoei    (501) staff       (20)     2908 2024-05-12 10:51:41.000000 pyboiler_anonoei-0.3.0/src/pyboiler/hml.py
--rwxrwx---   0 anonoei    (501) staff       (20)     1103 2024-05-12 10:24:59.000000 pyboiler_anonoei-0.3.0/src/pyboiler/hson.py
--rwxrwx---   0 anonoei    (501) staff       (20)     2358 2024-05-17 23:04:07.000000 pyboiler_anonoei-0.3.0/src/pyboiler/imports.py
--rwxrwx---   0 anonoei    (501) staff       (20)     3464 2024-05-19 23:23:53.000000 pyboiler_anonoei-0.3.0/src/pyboiler/logger.py
--rwxrwx---   0 anonoei    (501) staff       (20)     2597 2024-05-19 23:08:07.000000 pyboiler_anonoei-0.3.0/src/pyboiler/logging.py
--rwxrwx---   0 anonoei    (501) staff       (20)      571 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.3.0/src/pyboiler/platform.py
--rwxrwx---   0 anonoei    (501) staff       (20)      594 2024-05-12 10:40:35.000000 pyboiler_anonoei-0.3.0/src/pyboiler/profiler.py
--rwxrwx---   0 anonoei    (501) staff       (20)     3531 2024-05-12 13:29:41.000000 pyboiler_anonoei-0.3.0/src/pyboiler/settings.py
--rwxrwx---   0 anonoei    (501) staff       (20)     1893 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.3.0/src/pyboiler/version.py
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-19 23:33:27.478149 pyboiler_anonoei-0.3.0/src/pyboiler_anonoei.egg-info/
--rw-r--r--   0 anonoei    (501) staff       (20)     1355 2024-05-19 23:33:27.000000 pyboiler_anonoei-0.3.0/src/pyboiler_anonoei.egg-info/PKG-INFO
--rwxrwx---   0 anonoei    (501) staff       (20)     1141 2024-05-19 23:33:27.000000 pyboiler_anonoei-0.3.0/src/pyboiler_anonoei.egg-info/SOURCES.txt
--rwxrwx---   0 anonoei    (501) staff       (20)        1 2024-05-19 23:33:27.000000 pyboiler_anonoei-0.3.0/src/pyboiler_anonoei.egg-info/dependency_links.txt
--rwxrwx---   0 anonoei    (501) staff       (20)       46 2024-05-19 23:33:27.000000 pyboiler_anonoei-0.3.0/src/pyboiler_anonoei.egg-info/requires.txt
--rwxrwx---   0 anonoei    (501) staff       (20)        9 2024-05-19 23:33:27.000000 pyboiler_anonoei-0.3.0/src/pyboiler_anonoei.egg-info/top_level.txt
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-19 23:33:27.477801 pyboiler_anonoei-0.3.0/tests/
--rwxrwx---   0 anonoei    (501) staff       (20)      306 2024-05-12 23:16:15.000000 pyboiler_anonoei-0.3.0/tests/test_changelog.py
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-21 06:34:45.925836 pyboiler_anonoei-0.3.1/
+-rwxrwx---   0 anonoei    (501) staff       (20)     1051 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.3.1/LICENSE
+-rw-r--r--   0 anonoei    (501) staff       (20)     1355 2024-05-21 06:34:45.925504 pyboiler_anonoei-0.3.1/PKG-INFO
+-rwxrwx---   0 anonoei    (501) staff       (20)      281 2024-05-12 13:44:40.000000 pyboiler_anonoei-0.3.1/README.md
+-rwxrwx---   0 anonoei    (501) staff       (20)     1423 2024-05-21 06:33:59.000000 pyboiler_anonoei-0.3.1/pyproject.toml
+-rw-r--r--   0 anonoei    (501) staff       (20)       38 2024-05-21 06:34:45.925891 pyboiler_anonoei-0.3.1/setup.cfg
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-21 06:34:45.914982 pyboiler_anonoei-0.3.1/src/
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-21 06:34:45.920032 pyboiler_anonoei-0.3.1/src/pyboiler/
+-rwxrwx---   0 anonoei    (501) staff       (20)      813 2024-05-21 06:33:59.000000 pyboiler_anonoei-0.3.1/src/pyboiler/__init__.py
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-21 06:34:45.920317 pyboiler_anonoei-0.3.1/src/pyboiler/_internal/
+-rwxrwx---   0 anonoei    (501) staff       (20)        0 2024-05-17 22:45:41.000000 pyboiler_anonoei-0.3.1/src/pyboiler/_internal/__init__.py
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-21 06:34:45.921179 pyboiler_anonoei-0.3.1/src/pyboiler/_internal/color/
+-rwxrwx---   0 anonoei    (501) staff       (20)       48 2024-05-18 00:12:37.000000 pyboiler_anonoei-0.3.1/src/pyboiler/_internal/color/__init__.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     2474 2024-05-19 22:15:06.000000 pyboiler_anonoei-0.3.1/src/pyboiler/_internal/color/colors.py
+-rw-r--r--   0 anonoei    (501) staff       (20)      272 2024-05-19 21:50:23.000000 pyboiler_anonoei-0.3.1/src/pyboiler/_internal/color/config.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     1032 2024-05-19 21:38:25.000000 pyboiler_anonoei-0.3.1/src/pyboiler/_internal/color/parse.py
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-21 06:34:45.923124 pyboiler_anonoei-0.3.1/src/pyboiler/_internal/log/
+-rwxrwx---   0 anonoei    (501) staff       (20)      256 2024-05-18 09:15:43.000000 pyboiler_anonoei-0.3.1/src/pyboiler/_internal/log/__init__.py
+-rwxrwx---   0 anonoei    (501) staff       (20)      416 2024-05-19 22:46:14.000000 pyboiler_anonoei-0.3.1/src/pyboiler/_internal/log/config.py
+-rwxrwx---   0 anonoei    (501) staff       (20)      478 2024-05-18 02:02:44.000000 pyboiler_anonoei-0.3.1/src/pyboiler/_internal/log/filter.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     3836 2024-05-19 22:17:46.000000 pyboiler_anonoei-0.3.1/src/pyboiler/_internal/log/format.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     4019 2024-05-21 06:07:40.000000 pyboiler_anonoei-0.3.1/src/pyboiler/_internal/log/handler.py
+-rwxrwx---   0 anonoei    (501) staff       (20)      610 2024-05-19 19:07:04.000000 pyboiler_anonoei-0.3.1/src/pyboiler/_internal/log/inspect.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     1200 2024-05-19 21:55:02.000000 pyboiler_anonoei-0.3.1/src/pyboiler/_internal/log/level.py
+-rw-r--r--   0 anonoei    (501) staff       (20)      918 2024-05-21 06:33:07.000000 pyboiler_anonoei-0.3.1/src/pyboiler/_internal/log/queue.py
+-rwxrwx---   0 anonoei    (501) staff       (20)      517 2024-05-18 09:40:31.000000 pyboiler_anonoei-0.3.1/src/pyboiler/_internal/log/record.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     1331 2024-05-12 23:15:42.000000 pyboiler_anonoei-0.3.1/src/pyboiler/changelog.py
+-rwxrwx---   0 anonoei    (501) staff       (20)       74 2024-05-18 00:12:59.000000 pyboiler_anonoei-0.3.1/src/pyboiler/color.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     2464 2024-05-21 04:48:56.000000 pyboiler_anonoei-0.3.1/src/pyboiler/config.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     1041 2024-05-17 18:25:19.000000 pyboiler_anonoei-0.3.1/src/pyboiler/decor.py
+-rwxrwx---   0 anonoei    (501) staff       (20)      660 2024-05-12 23:46:14.000000 pyboiler_anonoei-0.3.1/src/pyboiler/error.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     4227 2024-05-19 23:26:23.000000 pyboiler_anonoei-0.3.1/src/pyboiler/generic.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     2908 2024-05-12 10:51:41.000000 pyboiler_anonoei-0.3.1/src/pyboiler/hml.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     1103 2024-05-12 10:24:59.000000 pyboiler_anonoei-0.3.1/src/pyboiler/hson.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     2358 2024-05-17 23:04:07.000000 pyboiler_anonoei-0.3.1/src/pyboiler/imports.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     3464 2024-05-21 06:10:23.000000 pyboiler_anonoei-0.3.1/src/pyboiler/logger.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     2527 2024-05-21 06:34:27.000000 pyboiler_anonoei-0.3.1/src/pyboiler/logging.py
+-rwxrwx---   0 anonoei    (501) staff       (20)      571 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.3.1/src/pyboiler/platform.py
+-rwxrwx---   0 anonoei    (501) staff       (20)      594 2024-05-12 10:40:35.000000 pyboiler_anonoei-0.3.1/src/pyboiler/profiler.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     3531 2024-05-12 13:29:41.000000 pyboiler_anonoei-0.3.1/src/pyboiler/settings.py
+-rwxrwx---   0 anonoei    (501) staff       (20)     1893 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.3.1/src/pyboiler/version.py
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-21 06:34:45.924666 pyboiler_anonoei-0.3.1/src/pyboiler_anonoei.egg-info/
+-rw-r--r--   0 anonoei    (501) staff       (20)     1355 2024-05-21 06:34:45.000000 pyboiler_anonoei-0.3.1/src/pyboiler_anonoei.egg-info/PKG-INFO
+-rwxrwx---   0 anonoei    (501) staff       (20)     1177 2024-05-21 06:34:45.000000 pyboiler_anonoei-0.3.1/src/pyboiler_anonoei.egg-info/SOURCES.txt
+-rwxrwx---   0 anonoei    (501) staff       (20)        1 2024-05-21 06:34:45.000000 pyboiler_anonoei-0.3.1/src/pyboiler_anonoei.egg-info/dependency_links.txt
+-rwxrwx---   0 anonoei    (501) staff       (20)       46 2024-05-21 06:34:45.000000 pyboiler_anonoei-0.3.1/src/pyboiler_anonoei.egg-info/requires.txt
+-rwxrwx---   0 anonoei    (501) staff       (20)        9 2024-05-21 06:34:45.000000 pyboiler_anonoei-0.3.1/src/pyboiler_anonoei.egg-info/top_level.txt
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-21 06:34:45.924421 pyboiler_anonoei-0.3.1/tests/
+-rwxrwx---   0 anonoei    (501) staff       (20)      306 2024-05-12 23:16:15.000000 pyboiler_anonoei-0.3.1/tests/test_changelog.py
```

### Comparing `pyboiler_anonoei-0.3.0/LICENSE` & `pyboiler_anonoei-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.3.0/PKG-INFO` & `pyboiler_anonoei-0.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyboiler_anonoei
-Version: 0.3.0
+Version: 0.3.1
 Summary: Various generic python helpers so I don't keep rewriting them
 Author-email: Anonoei <dev@anonoei.com>
 Project-URL: Homepage, https://github.com/anonoei/pyboiler
 Project-URL: Documentation, https://anonoei.github.io/pyboiler/
 Project-URL: Repository, https://github.com/Anonoei/pyboiler.git
 Project-URL: Issues, https://github.com/Anonoei/pyboiler/issues
 Project-URL: Source, https://github.com/anonoei/pyboiler
```

### Comparing `pyboiler_anonoei-0.3.0/pyproject.toml` & `pyboiler_anonoei-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyboiler_anonoei"
-version = "0.3.0"
+version = "0.3.1"
 description = "Various generic python helpers so I don't keep rewriting them"
 dependencies = []
 requires-python = ">=3.6"
 authors = [
     {name = "Anonoei", email="dev@anonoei.com"}
 ]
 readme = "README.md"
@@ -31,15 +31,15 @@
 Issues = "https://github.com/Anonoei/pyboiler/issues"
 Source = "https://github.com/anonoei/pyboiler"
 
 [project.optional-dependencies]
 dev = ["twine", "build", "black", "bumpver", "pytest", "pdoc3"]
 
 [tool.bumpver]
-current_version = "0.3.0"
+current_version = "0.3.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 pre_commit_hook = ""
 post_commit_hook = ""
 commit = true
```

### Comparing `pyboiler_anonoei-0.3.0/src/pyboiler/__init__.py` & `pyboiler_anonoei-0.3.1/src/pyboiler/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
  Imports all files in src/pyboiler/* so they can be imported as
  `pyboiler.config`
 """
 
 import pathlib
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 __author__ = "Anonoei <dev@anonoei.com>"
 init_run = False
 
 
 def __init(_val=[]):
     """Import all files in `import_path`"""
     if _val:
```

### Comparing `pyboiler_anonoei-0.3.0/src/pyboiler/_internal/color/colors.py` & `pyboiler_anonoei-0.3.1/src/pyboiler/_internal/color/colors.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.3.0/src/pyboiler/_internal/color/parse.py` & `pyboiler_anonoei-0.3.1/src/pyboiler/_internal/color/parse.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.3.0/src/pyboiler/_internal/log/format.py` & `pyboiler_anonoei-0.3.1/src/pyboiler/_internal/log/format.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.3.0/src/pyboiler/_internal/log/handler.py` & `pyboiler_anonoei-0.3.1/src/pyboiler/_internal/log/handler.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 """Wrap python.logging Handlers"""
 
 import sys
+import pathlib
+import socket
+import random
 
 from ...generic import slot_storage
 from .format import Formatter, default, colored
 from .level import Level
 from .record import Record
 
+from .queue import Queue
+
 
 class Handler(slot_storage):
-    """Handle log records"""
+    """Handle logs"""
 
-    __slots__ = ("_level", "_format", "_io", "_meta")
+    __slots__ = ("_level", "_format")
 
     def __init__(self, level=Level.NOTSET):
         self._level = level
         self._format = default
         self._io = None
         try:
             self._meta
@@ -29,100 +34,132 @@
         return type(self).name()
 
     def __repr__(self) -> str:
         return f"<{type(self).__name__}: {self._level}>"
 
     @classmethod
     def name(cls):
+        """Get the base name of this handler"""
         return cls.__name__[:-7].lower()
 
     @property
     def level(self):
+        """Get/Set this handler's level"""
         return self._level
 
     @level.setter
     def level(self, lvl: Level):
         self._level = Level.get(lvl)
 
     @property
     def formatter(self):
+        """Get/Set this handler's formatter"""
         return self._format
 
     @formatter.setter
     def formatter(self, val: Formatter):
         self._format = val
 
     def _handle(self, record: Record):
         if self.level < record.level:
             return False
         return True
 
-    def handle(self, record: Record): ...
-
-    def close(self): ...
+    def handle(self, record: Record):
+        """Handle a log record"""
+        ...
 
     def format(self, record):
+        """Format a log record"""
         return self._format.format(record)
 
 
 class StreamHandler(Handler):
-    """Writes log records to a stream"""
+    """Writes logs to stream"""
+
+    __slots__ = ("_level", "_format", "_io")
 
     def __init__(self, stream, level: Level):
         super().__init__(level)
         self._io = stream
 
-    def flush(self):
-        self._io.flush()
-
     def handle(self, record):
         if not self._handle(record):
             return
         msg = self.format(record)
         self._io.write(msg + "\n")
-        self.flush()
+        self._io.flush()
 
 
 class FileHandler(StreamHandler):
-    """Writes log records to a file"""
+    """Writes logs to file"""
 
-    def __init__(self, filepath, level: Level, mode="a", encoding="UTF-8"):
-        self._io = None
-        self.meta = {}
-        self.meta["filepath"] = filepath
-        self.meta["mode"] = mode
-        self.meta["encoding"] = encoding
-        self.meta["open"] = False
-        super().__init__(self._open(), level)
-
-    def _open(self):
-        _io = self._io
-        if not self.meta["open"]:
-            _io = open(
-                self.meta["filepath"],
-                mode=self.meta["mode"],
-                encoding=self.meta["encoding"],
-            )
-            self.meta["open"] = True
-        return _io
+    __slots__ = ("_level", "_format", "_io")
 
-    def _close(self):
+    def __init__(
+        self, filepath: pathlib.Path, level: Level, mode="a", encoding="UTF-8"
+    ):
+        if not filepath.exists():
+            mode = "w"
+        _io = filepath.open(mode=mode, encoding=encoding)
+        super().__init__(_io, level)
+
+    def close(self):
+        Queue().stop()
         self._io.close()
-        self.meta["open"] = False
+
+    def handle(self, record):
+        sup = super()
+        Queue().add([lambda s=sup, r=record: sup.handle(record)])
+
+
+class OverwriteFileHandler(FileHandler):
+    """Write logs to file and overwrite them if they exist"""
+
+    __slots__ = ("_level", "_format", "_io")
+
+    def __init__(self, filepath: pathlib.Path, level: Level, encoding="UTF-8"):
+        super().__init__(filepath, level, "w", encoding)
 
 
 class StdoutHandler(StreamHandler):
+    """Write logs to stdout"""
+
+    __slots__ = ("_level", "_format", "_io")
+
     def __init__(self, level: Level):
         super().__init__(sys.stdout, level)
         self._format = colored
 
 
 class StderrHandler(StreamHandler):
+    """Write logs to stderr"""
+
+    __slots__ = ("_level", "_format", "_io")
+
     def __init__(self, level: Level):
         super().__init__(sys.stderr, level)
 
 
+class SocketHandler(Handler):
+    __slots__ = ("_level", "_format", "_socket", "_address", "_encoding")
+
+    def __init__(self, host, port, level: Level, encoding="UTF-8"):
+        self._level = level
+        self._format = default
+        self._address = (host, port)
+        self._socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        self._socket.connect(self._address)
+        self._encoding = encoding
+
+    def handle(self, record: Record):
+        if not self._handle(record):
+            return
+        msg = self.format(record)
+        self._socket.send(msg.encode(self._encoding))
+
+
 handlers = {
     k[:-7].lower(): v
     for k, v in globals().items()
     if not k == "Handler" and k.endswith("Handler")
 }
```

### Comparing `pyboiler_anonoei-0.3.0/src/pyboiler/_internal/log/inspect.py` & `pyboiler_anonoei-0.3.1/src/pyboiler/_internal/log/inspect.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.3.0/src/pyboiler/_internal/log/level.py` & `pyboiler_anonoei-0.3.1/src/pyboiler/_internal/log/level.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.3.0/src/pyboiler/_internal/log/record.py` & `pyboiler_anonoei-0.3.1/src/pyboiler/_internal/log/record.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.3.0/src/pyboiler/changelog.py` & `pyboiler_anonoei-0.3.1/src/pyboiler/changelog.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.3.0/src/pyboiler/config.py` & `pyboiler_anonoei-0.3.1/src/pyboiler/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,18 +10,21 @@
 
 Add your own global configuration variables
 ```python
 config().MY_VARIABLE = "Hello, world!"
 ```
 """
 
+import sys
+import os
 import pathlib
 import subprocess
 
 from .imports import get_locals
+from ._internal.log.inspect import meta
 
 
 class config:
     """Global configuration, not intended to be modified by users"""
 
     __instance = None
 
@@ -61,17 +64,20 @@
 
         for k in get_locals(self, ("init", "json")):
             fmt[k] = getattr(self, k)
         return fmt
 
     def _init_path_root(self) -> pathlib.Path:
         """Initialize PATH_ROOT to the toplevel of the git repo"""
-        fpath = subprocess.getoutput("git rev-parse --show-toplevel")
+        mod_file = pathlib.Path(os.path.dirname(sys.argv[0])).absolute()
+        fpath = subprocess.getoutput(
+            f"cd {str(mod_file)} && git rev-parse --show-toplevel"
+        )
         if "fatal:" in fpath:
-            fpath = pathlib.Path(__file__).parent.parent
+            fpath = mod_file
         else:
             fpath = pathlib.Path(fpath)
         return fpath
 
     def _init_sys_plat(self):
         """Initialize SYS_PLAT to a pyboiler.platform.Platform enum"""
         from .platform import Platform
```

### Comparing `pyboiler_anonoei-0.3.0/src/pyboiler/decor.py` & `pyboiler_anonoei-0.3.1/src/pyboiler/decor.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.3.0/src/pyboiler/error.py` & `pyboiler_anonoei-0.3.1/src/pyboiler/error.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.3.0/src/pyboiler/generic.py` & `pyboiler_anonoei-0.3.1/src/pyboiler/generic.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.3.0/src/pyboiler/hml.py` & `pyboiler_anonoei-0.3.1/src/pyboiler/hml.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.3.0/src/pyboiler/hson.py` & `pyboiler_anonoei-0.3.1/src/pyboiler/hson.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.3.0/src/pyboiler/imports.py` & `pyboiler_anonoei-0.3.1/src/pyboiler/imports.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.3.0/src/pyboiler/logger.py` & `pyboiler_anonoei-0.3.1/src/pyboiler/logger.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.3.0/src/pyboiler/logging.py` & `pyboiler_anonoei-0.3.1/src/pyboiler/logging.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,10 @@
-"""Wrap python.logging in an interface I prefer"""
+"""Threaded logger with color support"""
 
-import queue
-
-from ._internal.log import Handler, Level, Record, config, handlers
-from .generic import storage
-
-logstore = storage()
-logstore.queue = queue.Queue()
+from ._internal.log import Handler, Level, Record, handlers
 
 
 class logging:
 
     __slots__ = ("name", "_level", "handlers", "disabled")
 
     def __init__(self, name, level):
@@ -53,14 +47,15 @@
     def rm_handler(self, hdlr):
         """Remove a handler"""
         if isinstance(hdlr, str):
             hdlr = handlers[hdlr]
         self.handlers.pop(hdlr)
 
     def ls_handlers(self):
+        """Return all available handlers"""
         return self.handlers
 
     def trace(self, msg):
         """Log trace"""
         self._log(Level.TRACE, msg)
 
     def debug(self, msg):
```

### Comparing `pyboiler_anonoei-0.3.0/src/pyboiler/platform.py` & `pyboiler_anonoei-0.3.1/src/pyboiler/platform.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.3.0/src/pyboiler/profiler.py` & `pyboiler_anonoei-0.3.1/src/pyboiler/profiler.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.3.0/src/pyboiler/settings.py` & `pyboiler_anonoei-0.3.1/src/pyboiler/settings.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.3.0/src/pyboiler/version.py` & `pyboiler_anonoei-0.3.1/src/pyboiler/version.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.3.0/src/pyboiler_anonoei.egg-info/PKG-INFO` & `pyboiler_anonoei-0.3.1/src/pyboiler_anonoei.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyboiler_anonoei
-Version: 0.3.0
+Version: 0.3.1
 Summary: Various generic python helpers so I don't keep rewriting them
 Author-email: Anonoei <dev@anonoei.com>
 Project-URL: Homepage, https://github.com/anonoei/pyboiler
 Project-URL: Documentation, https://anonoei.github.io/pyboiler/
 Project-URL: Repository, https://github.com/Anonoei/pyboiler.git
 Project-URL: Issues, https://github.com/Anonoei/pyboiler/issues
 Project-URL: Source, https://github.com/anonoei/pyboiler
```

### Comparing `pyboiler_anonoei-0.3.0/src/pyboiler_anonoei.egg-info/SOURCES.txt` & `pyboiler_anonoei-0.3.1/src/pyboiler_anonoei.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 src/pyboiler/_internal/log/__init__.py
 src/pyboiler/_internal/log/config.py
 src/pyboiler/_internal/log/filter.py
 src/pyboiler/_internal/log/format.py
 src/pyboiler/_internal/log/handler.py
 src/pyboiler/_internal/log/inspect.py
 src/pyboiler/_internal/log/level.py
+src/pyboiler/_internal/log/queue.py
 src/pyboiler/_internal/log/record.py
 src/pyboiler_anonoei.egg-info/PKG-INFO
 src/pyboiler_anonoei.egg-info/SOURCES.txt
 src/pyboiler_anonoei.egg-info/dependency_links.txt
 src/pyboiler_anonoei.egg-info/requires.txt
 src/pyboiler_anonoei.egg-info/top_level.txt
 tests/test_changelog.py
```

