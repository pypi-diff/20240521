# Comparing `tmp/play3slib-0.0.1.tar.gz` & `tmp/play3slib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "play3slib-0.0.1.tar", last modified: Mon May 20 08:10:48 2024, max compression
+gzip compressed data, was "play3slib-0.0.2.tar", last modified: Tue May 21 01:20:51 2024, max compression
```

## Comparing `play3slib-0.0.1.tar` & `play3slib-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 08:10:48.567481 play3slib-0.0.1/
--rw-rw-rw-   0        0        0       33 2024-05-20 05:32:02.000000 play3slib-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      613 2024-05-20 08:10:48.565671 play3slib-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       34 2024-05-20 05:31:54.000000 play3slib-0.0.1/README.md
--rw-rw-rw-   0        0        0      487 2024-05-20 08:06:44.000000 play3slib-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-20 08:10:48.568339 play3slib-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      802 2024-05-20 08:10:20.000000 play3slib-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-20 08:10:48.317776 play3slib-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-20 08:10:48.563497 play3slib-0.0.1/src/play3slib.egg-info/
--rw-rw-rw-   0        0        0      613 2024-05-20 08:10:48.000000 play3slib-0.0.1/src/play3slib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2024-05-20 08:10:48.000000 play3slib-0.0.1/src/play3slib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 08:10:48.000000 play3slib-0.0.1/src/play3slib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 08:10:48.000000 play3slib-0.0.1/src/play3slib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 01:20:51.311855 play3slib-0.0.2/
+-rw-rw-rw-   0        0        0       33 2024-05-20 05:32:02.000000 play3slib-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      605 2024-05-21 01:20:51.307854 play3slib-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       34 2024-05-20 05:31:54.000000 play3slib-0.0.2/README.md
+-rw-rw-rw-   0        0        0      483 2024-05-21 01:20:22.000000 play3slib-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 01:20:51.311855 play3slib-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      794 2024-05-21 01:20:22.000000 play3slib-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 01:20:51.275862 play3slib-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-21 01:20:51.305909 play3slib-0.0.2/src/play3slib.egg-info/
+-rw-rw-rw-   0        0        0      605 2024-05-21 01:20:51.000000 play3slib-0.0.2/src/play3slib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2024-05-21 01:20:51.000000 play3slib-0.0.2/src/play3slib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 01:20:51.000000 play3slib-0.0.2/src/play3slib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 01:20:51.000000 play3slib-0.0.2/src/play3slib.egg-info/top_level.txt
```

### Comparing `play3slib-0.0.1/setup.py` & `play3slib-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="play3slib",
-    version="0.0.1",
+    version="0.0.2",
     author="chaoren2",
     author_email="chaoren2@naver.com",
     description="Play3s's library",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/play3s/ctv_protector",
+    url="https://github.com/play3s/play3slib",
     project_urls={
-        "Bug Tracker": "https://github.com/play3s/ctv_protector",
+        "Bug Tracker": "https://github.com/play3s/play3slib",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
```

