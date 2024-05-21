# Comparing `tmp/play3slib-0.0.3.tar.gz` & `tmp/play3slib-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "play3slib-0.0.3.tar", last modified: Tue May 21 01:30:22 2024, max compression
+gzip compressed data, was "play3slib-0.0.4.tar", last modified: Tue May 21 04:03:54 2024, max compression
```

## Comparing `play3slib-0.0.3.tar` & `play3slib-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 01:30:22.593560 play3slib-0.0.3/
--rw-rw-rw-   0        0        0       33 2024-05-20 05:32:02.000000 play3slib-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0      605 2024-05-21 01:30:22.590557 play3slib-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       34 2024-05-20 05:31:54.000000 play3slib-0.0.3/README.md
--rw-rw-rw-   0        0        0      483 2024-05-21 01:28:45.000000 play3slib-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-21 01:30:22.594561 play3slib-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      794 2024-05-21 01:28:45.000000 play3slib-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-21 01:30:22.557559 play3slib-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-21 01:30:22.571557 play3slib-0.0.3/src/play3slib/
--rw-rw-rw-   0        0        0        0 2024-05-20 05:27:41.000000 play3slib-0.0.3/src/play3slib/__init__.py
--rw-rw-rw-   0        0        0       40 2024-05-20 05:30:32.000000 play3slib-0.0.3/src/play3slib/mod1.py
-drwxrwxrwx   0        0        0        0 2024-05-21 01:30:22.588558 play3slib-0.0.3/src/play3slib.egg-info/
--rw-rw-rw-   0        0        0      605 2024-05-21 01:30:22.000000 play3slib-0.0.3/src/play3slib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2024-05-21 01:30:22.000000 play3slib-0.0.3/src/play3slib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 01:30:22.000000 play3slib-0.0.3/src/play3slib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-21 01:30:22.000000 play3slib-0.0.3/src/play3slib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 04:03:54.103030 play3slib-0.0.4/
+-rw-rw-rw-   0        0        0       33 2024-05-20 05:32:02.000000 play3slib-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      605 2024-05-21 04:03:54.100030 play3slib-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       34 2024-05-20 05:31:54.000000 play3slib-0.0.4/README.md
+-rw-rw-rw-   0        0        0      483 2024-05-21 04:02:53.000000 play3slib-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 04:03:54.103030 play3slib-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      794 2024-05-21 04:02:50.000000 play3slib-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 04:03:53.981927 play3slib-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-21 04:03:54.004926 play3slib-0.0.4/src/play3slib/
+-rw-rw-rw-   0        0        0        0 2024-05-20 05:27:41.000000 play3slib-0.0.4/src/play3slib/__init__.py
+-rw-rw-rw-   0        0        0       88 2024-05-21 03:58:42.000000 play3slib-0.0.4/src/play3slib/mod1.py
+drwxrwxrwx   0        0        0        0 2024-05-21 04:03:54.099028 play3slib-0.0.4/src/play3slib.egg-info/
+-rw-rw-rw-   0        0        0      605 2024-05-21 04:03:53.000000 play3slib-0.0.4/src/play3slib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2024-05-21 04:03:53.000000 play3slib-0.0.4/src/play3slib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 04:03:53.000000 play3slib-0.0.4/src/play3slib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-21 04:03:53.000000 play3slib-0.0.4/src/play3slib.egg-info/top_level.txt
```

### Comparing `play3slib-0.0.3/PKG-INFO` & `play3slib-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: play3slib
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small example package
 Home-page: https://github.com/play3s/play3slib
 Author: chaoren2
 Author-email: chaoren2 <chaoren2@naver.com>
 Project-URL: Homepage, https://github.com/play3s/play3slib
 Project-URL: Issues, https://github.com/play3s/play3slib/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `play3slib-0.0.3/setup.py` & `play3slib-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="play3slib",
-    version="0.0.3",
+    version="0.0.4",
     author="chaoren2",
     author_email="chaoren2@naver.com",
     description="Play3s's library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/play3s/play3slib",
     project_urls={
```

### Comparing `play3slib-0.0.3/src/play3slib.egg-info/PKG-INFO` & `play3slib-0.0.4/src/play3slib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: play3slib
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small example package
 Home-page: https://github.com/play3s/play3slib
 Author: chaoren2
 Author-email: chaoren2 <chaoren2@naver.com>
 Project-URL: Homepage, https://github.com/play3s/play3slib
 Project-URL: Issues, https://github.com/play3s/play3slib/issues
 Classifier: Programming Language :: Python :: 3
```

